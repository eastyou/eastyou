# 你好，我是 eastyou

把重复劳动交给命令行，用 Python 标准库写零依赖的小工具。

所有项目均以 [MIT](https://opensource.org/licenses/MIT) 协议开源，欢迎 Issue 与 PR。

## 项目一览

| 项目 | 一句话说明 | 技术点 |
| --- | --- | --- |
| [zh-text-stats](https://github.com/eastyou/zh-text-stats) | 中文文本统计：字数、标点、段落、阅读时长、高频词 | 正则、Unicode、argparse |
| [md-link-check](https://github.com/eastyou/md-link-check) | Markdown 死链检查：本地路径、标题锚点、外部链接 | 并发请求、锚点解析 |
| [srt-tool](https://github.com/eastyou/srt-tool) | SRT 字幕体检、平移、变速、转 WebVTT | 时间轴运算、边界处理 |
| [portpeek](https://github.com/eastyou/portpeek) | 跨平台端口占用查询，看清哪个进程占了端口 | 子进程、多平台适配 |
| [jsonl-csv](https://github.com/eastyou/jsonl-csv) | JSONL 与 CSV 双向流式转换，适合大文件 | 流式 IO、CSV 转义 |
| [miniredis](https://github.com/eastyou/miniredis) | 用 asyncio 从零实现的迷你 Redis | RESP2、TTL、AOF |
| [pure-raytracer](https://github.com/eastyou/pure-raytracer) | 纯 Python 光线追踪渲染器 | 路径追踪、手写 PNG |
| [minihttpd](https://github.com/eastyou/minihttpd) | asyncio 版 HTTP/1.1 框架与服务器 | 路由、中间件、keep-alive |
| [cronit](https://github.com/eastyou/cronit) | cron 表达式校验与下次执行时间 | 解析器、时间搜索 |
| [classseat](https://github.com/eastyou/classseat) | 班级座位表：前排优先、固定座位、需分开，输出可打印 A4 | 约束满足、多轮随机重试 |
| [classpick](https://github.com/eastyou/classpick) | 课堂随机点名与分组，一轮不重复、可排除请假 | 随机抽样、状态持久化 |
| [gradekit](https://github.com/eastyou/gradekit) | 成绩分析：各科平均分、及格率与分数段分布 | CSV 校验、统计、SVG 图表 |
| [chemviz](https://github.com/eastyou/chemviz) | 初中化学可视化：元素周期表、原子结构、分子模型与方程式配平 | SVG 绘图、分数高斯消元 |
| [physicsviz](https://github.com/eastyou/physicsviz) | 初中物理可视化：凸透镜光路、串并联电路、运动图像 | 成像公式、电路计算、SVG |
| [mathviz](https://github.com/eastyou/mathviz) | 初中数学可视化：函数图像、勾股定理、频数分布直方图 | 函数特征、SVG 坐标、统计 |
| [paperkit](https://github.com/eastyou/paperkit) | 试卷生成器：题库 CSV 生成可打印试卷与答案页 | CSV 校验、选项重排、打印排版 |
| [wordcard](https://github.com/eastyou/wordcard) | 英语单词默写纸：单词表 CSV 生成 A4 默写卡 | 模式切换、随机排序、打印排版 |
| [classtimer](https://github.com/eastyou/classtimer) | 课堂倒计时：预设时间、全屏显示、结束提示音 | 单文件 HTML、原生 JS、无依赖 |

---

## zh-text-stats

[![CI](https://github.com/eastyou/zh-text-stats/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/zh-text-stats/actions/workflows/ci.yml)

`wc -m` 对中文并不友好。这个工具把汉字、英文单词、数字、标点、段落分别统计，估算阅读时长，并提炼高频词，支持 JSON 输出。

```bash
zhstats article.txt --top 5
cat article.txt | zhstats --stdin --json
```

## md-link-check

[![CI](https://github.com/eastyou/md-link-check/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/md-link-check/actions/workflows/ci.yml)

文档一多就容易留下死链。扫描所有 Markdown，跳过代码块，检查本地路径、`#锚点` 和外部链接，发现问题时退出码为 1，可直接接入 CI。

```bash
mdlink docs --offline
mdlink . --json --concurrency 16
```

## srt-tool

[![CI](https://github.com/eastyou/srt-tool/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/srt-tool/actions/workflows/ci.yml)

字幕整体快了或慢了，不必打开图形软件。支持体检、整体平移、按倍速缩放、转 WebVTT，越界的字幕会自动裁剪或丢弃并给出统计。

```bash
srttool check ep01.srt
srttool shift ep01.srt -s -1.5 -o ep01.fixed.srt
srttool speed ep01.srt -r 1.25 -i
```

## portpeek

[![CI](https://github.com/eastyou/portpeek/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/portpeek/actions/workflows/ci.yml)

`Address already in use` 的排查工具。macOS 用 `lsof`，Linux 优先 `ss`，Windows 用 `netstat` + `tasklist`，统一成一张表；`--check` 用退出码告诉脚本端口是否空闲。

```bash
portpeek 3000 8080
portpeek --check 3000
```

## jsonl-csv

[![CI](https://github.com/eastyou/jsonl-csv/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/jsonl-csv/actions/workflows/ci.yml)

日志和模型输出常是 JSONL，Excel 和数据库更喜欢 CSV。边读边写，内存占用与文件大小无关；错误信息带行号，表头不一致会明确报错。

```bash
jsonlcsv to-csv -i events.jsonl > events.csv
jsonlcsv to-jsonl -i events.csv --infer-types
```

## miniredis

[![CI](https://github.com/eastyou/miniredis/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/miniredis/actions/workflows/ci.yml)

用 asyncio 从零写的 Redis：RESP2 线协议、增量解析、四种数据结构、键过期、AOF 持久化。兼容官方 `redis-cli`，79 个测试覆盖协议分片、命令语义与真实 socket。

```bash
miniredis-server --port 6399 --aof data.aof
miniredis-cli SET greeting hello
```

## pure-raytracer

[![CI](https://github.com/eastyou/pure-raytracer/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/pure-raytracer/actions/workflows/ci.yml)

纯 Python 光线追踪渲染器：漫反射、金属、玻璃折射、软阴影、景深，并用 `zlib` + `struct` 手写 PNG 编码，零第三方依赖。

![渲染示例](https://raw.githubusercontent.com/eastyou/pure-raytracer/main/examples/demo.png)

```bash
raytrace -o render.png -W 800 -H 450 -s 32
```

## minihttpd

[![CI](https://github.com/eastyou/minihttpd/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/minihttpd/actions/workflows/ci.yml)

基于 asyncio 的迷你 HTTP/1.1 框架：`{param}` 路由、中间件、JSON 请求体、静态文件、HEAD、405 自动协商、keep-alive 与流水线，附带 57 个测试。

```python
from minihttpd.app import App
from minihttpd.response import Response

app = App()

@app.get("/hello/{name}")
async def hello(request, name: str) -> Response:
    return Response.json({"hello": name})
```

## cronit

[![CI](https://github.com/eastyou/cronit/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/cronit/actions/workflows/ci.yml)

cron 表达式工具：校验写法、翻译成中文、算出未来 N 次执行时间。支持范围、步长、逗号列表、英文缩写与 `@daily` 别名，能正确处理闰年 2 月 29 日。

```bash
cronit next "0 9 * * MON-FRI" -n 3
cronit explain "*/15 * * * *"
```

## classseat

[![CI](https://github.com/eastyou/classseat/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/classseat/actions/workflows/ci.yml)

给老师用的座位表生成器。近视的同学优先前排、个别同学固定座位、指定的两人不相邻，这些要求写进名单后一次生成 A4 横向座位表，可直接打印。

```bash
classseat -i 名单.csv --rows 6 --columns 7 --front-rows 2 -o 座位表.html
```

## classpick

[![CI](https://github.com/eastyou/classpick/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/classpick/actions/workflows/ci.yml)

课堂随机点名与分组。真正的随机抽样，可一次点多人；用状态文件保证一轮内不重复，点完自动开启新一轮；临时请假的同学可以排除。

```bash
classpick pick -i 名单.txt --state .classpick.json
classpick group -i 名单.txt -g 3
```

## gradekit

[![CI](https://github.com/eastyou/gradekit/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/gradekit/actions/workflows/ci.yml)

把 Excel 成绩表另存为 CSV，一条命令得到各科平均分、中位数、及格率、优秀率和分数段分布，并生成一页 A4 打印报告。缺考自动跳过，报告只含汇总数据，不出现个人排名。

```bash
gradekit -i 成绩.csv -o 报告.html --csv 统计.csv
```

## chemviz

[![CI](https://github.com/eastyou/chemviz/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/chemviz/actions/workflows/ci.yml)

初中化学可视化：前 20 号元素周期表、原子结构示意图、9 种常见分子模型，一页 A4 横向打印。命令行还能算相对分子质量，并用线性代数自动配平化学方程式。

```bash
chemviz html -o 化学可视化.html
chemviz mass "Ca(OH)2"
chemviz balance "Fe + O2 = Fe3O4"
```

## physicsviz

[![CI](https://github.com/eastyou/physicsviz/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/physicsviz/actions/workflows/ci.yml)

初中物理可视化：输入物距和焦距就画出凸透镜成像光路，输入电阻和电压就算串并联电路，输入速度和时间就画 s-t、v-t 图像，结果可汇总成打印页。

```bash
physicsviz lens -u 30 -f 10
physicsviz circuit -t series -r 10,20 -v 6
physicsviz motion -v 5 -t 10
physicsviz html -o 物理可视化.html
```

## mathviz

[![CI](https://github.com/eastyou/mathviz/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/mathviz/actions/workflows/ci.yml)

初中数学可视化：一次函数、二次函数、反比例函数的图像与关键点，勾股定理的三正方形面积图，以及带平均数和中位数的频数分布直方图。

```bash
mathviz linear -k 2 -b 1
mathviz quadratic -a 1 -b -2 -c -3
mathviz pythagoras -a 3 -b 4
mathviz html -o 数学可视化.html
```

## paperkit

[![CI](https://github.com/eastyou/paperkit/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/paperkit/actions/workflows/ci.yml)

试卷生成器：用 Excel 维护题库 CSV，一条命令生成可打印的 A4 试卷与答案页。支持选择题、填空题、打乱题目和选项，答案字母随选项同步重排。

```bash
paperkit -i 题库.csv -o 试卷.html --shuffle-questions --shuffle-options
```

## wordcard

[![CI](https://github.com/eastyou/wordcard/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/wordcard/actions/workflows/ci.yml)

英语单词默写纸：读单词表 CSV，生成看英文写中文、看中文写英文或英中交替的 A4 默写卡，可打乱顺序、切换 1~3 列，附答案页。

```bash
wordcard -i 单词.csv -o 默写纸.html --mode mixed --columns 2
```

## classtimer

[![CI](https://github.com/eastyou/classtimer/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/classtimer/actions/workflows/ci.yml)

课堂倒计时：生成单文件 HTML，双击即可全屏使用。预设 1/3/5/10 分钟，支持开始、暂停、重置、键盘快捷键和结束提示音，断网也能用。

```bash
classtimer -o 课堂计时.html --presets 1,3,5,10
```

---

## 开发约定

- 只依赖 Python 标准库，`pip install` 即可用
- 关键逻辑全部有单元测试，CI 覆盖 Python 3.9 ~ 3.13
- 输入校验与错误提示优先：文件不存在、编码错误、参数越界都会给出中文提示和明确退出码
- 提交信息遵循 Conventional Commits
