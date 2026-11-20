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
| [timetable](https://github.com/eastyou/timetable) | 课程表生成器：课程 CSV 生成可打印课程表，自动检测冲突 | 时间区间、周次交集、A4 横向布局 |
| [geoviz](https://github.com/eastyou/geoviz) | 世界时区换算：终端查时差，生成 24 小时带对照图 | 固定偏移、跨日计算、表格对齐 |
| [mindmap](https://github.com/eastyou/mindmap) | 缩进大纲转 SVG 思维导图，可投屏可打印 | 树布局、贝塞尔曲线、文字宽度估算 |
| [mathdrill](https://github.com/eastyou/mathdrill) | 口算题生成器：四则运算自由组合，自动去重，生成 A4 练习纸 | 随机生成、题目指纹、打印排版 |
| [labbook](https://github.com/eastyou/labbook) | 实验记录单：实验清单 CSV 生成可打印 A4 记录单 | CSV 校验、分隔符解析、打印排版 |
| [dutyrota](https://github.com/eastyou/dutyrota) | 值日轮值表：名单均衡轮转，自动标注日期并打印 | 均衡分配、同日去重、日期计算 |
| [tianzige](https://github.com/eastyou/tianzige) | 田字格练字帖：生字表生成 A4 字帖，支持描红与米字格 | 分页排版、CSS 格线、打印 |
| [clockdrill](https://github.com/eastyou/clockdrill) | 钟表练习纸：看钟面写时间、看时间画指针 | SVG 钟面、角度计算、答案页 |
| [wordsearch](https://github.com/eastyou/wordsearch) | 英语单词找词游戏：单词表生成字母网格与答案 | 网格放置、交叉校验、答案高亮 |
| [graphpaper](https://github.com/eastyou/graphpaper) | 方格纸 / 点阵纸 / 坐标纸生成器，A4 精确排版可直接打印 | SVG 网格、坐标刻度、毫米排版 |
| [nametag](https://github.com/eastyou/nametag) | 姓名桌牌：名单 CSV 生成 A4 折叠桌牌，前后两面镜像 | CSV 校验、旋转镜像、自适应字号 |
| [maze](https://github.com/eastyou/maze) | 迷宫生成器：完美迷宫配入口出口，可选答案页 | DFS 生成、BFS 求解、SVG 绘制 |
| [sudoku](https://github.com/eastyou/sudoku) | 数独生成器：唯一解、三档难度、可选答案页 | 位掩码回溯、MRV、唯一解校验 |
| [certkit](https://github.com/eastyou/certkit) | 奖状生成器：名单 CSV 生成 A4 横向可打印奖状 | CSV 编码识别、自适应字号、SVG 排版 |
| [readinglog](https://github.com/eastyou/readinglog) | 阅读记录表：书目 CSV 生成 A4 可打印表格 | CSV 校验、分页、打印排版 |
| [bingo](https://github.com/eastyou/bingo) | 课堂宾果卡：词表生成 A4 卡片与叫号单 | 随机分卡、去重校验、打印排版 |
| [flashcard](https://github.com/eastyou/flashcard) | 双向记忆卡：术语释义 CSV 生成正反面卡片 | 双面镜像、字号自适应、打印排版 |
| [attendance](https://github.com/eastyou/attendance) | 班级考勤表：名单生成整月 A4 横向表格 | 月份校验、周末标色、自动分页 |

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

## timetable

[![CI](https://github.com/eastyou/timetable/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/timetable/actions/workflows/ci.yml)

课程表生成器：用 Excel 维护课程 CSV，一条命令生成一页 A4 横向课程表。课块按真实时间比例绘制，同一天时间重叠且周次相交的课会被列出并用红框标出。

```bash
timetable -i 课程.csv -o 课程表.html --title "初二(3)班课程表"
```

## geoviz

[![CI](https://github.com/eastyou/geoviz/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/geoviz/actions/workflows/ci.yml)

世界时区换算：在终端一次查询多个城市，自动标注「前一天 / 次日」；也能生成一页 24 小时昼夜色带对照图，适合地理课讲时区和日界线。

```bash
geoviz convert --at "2026-11-21 12:00" --from 北京 --to 纽约,伦敦,东京
geoviz html --at "2026-11-21 12:00" --from 北京 -o 时区对照.html
```

## mindmap

[![CI](https://github.com/eastyou/mindmap/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/mindmap/actions/workflows/ci.yml)

把缩进大纲转换成 SVG 思维导图：空格或 Tab 表示层级，自动完成树形布局，输出单文件 HTML，可投屏、可打印。

```bash
mindmap -i 复习提纲.txt -o 思维导图.html --title "初中物理复习"
```

## mathdrill

[![CI](https://github.com/eastyou/mathdrill/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/mathdrill/actions/workflows/ci.yml)

口算题生成器：加、减、乘、除自由组合，数值范围和题目数量可调。减法不出负数，除法保证整除，加法和乘法会把 `3+5` 与 `5+3` 视为同一题去重。输出一页 A4 练习纸，附参考答案。

```bash
mathdrill --ops add,sub --max 20 --count 40 -o 口算练习.html
mathdrill --ops add,sub,mul,div --count 50 --seed 2026 -o 综合练习.html
```

## labbook

[![CI](https://github.com/eastyou/labbook/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/labbook/actions/workflows/ci.yml)

实验记录单生成器：用 Excel 维护实验清单 CSV，一条命令生成带目的、器材、步骤、安全提示和手写记录区的 A4 记录单。表头缺失、名称为空会指出具体行号。

```bash
labbook -i 实验清单.csv -o 实验记录单.html --rows 6
```

## dutyrota

[![CI](https://github.com/eastyou/dutyrota/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/dutyrota/actions/workflows/ci.yml)

值日轮值表生成器：名单交给它，指定周数、每周天数和每天人数，自动均衡轮转。任意两人值日次数最多相差 1 次，同一天不会重复，给出起始日期还能标出每周的具体日期。

```bash
dutyrota -i 名单.txt -o 值日表.html --weeks 4 --per-day 2 --start 2026-11-23
```

## tianzige

[![CI](https://github.com/eastyou/tianzige/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/tianzige/actions/workflows/ci.yml)

田字格练字帖生成器：输入生字，自动排成多页 A4 字帖。支持田字格、米字格和方格，每行前几个格子浅色描红，其余留白，自动分页并标注页码。

```bash
tianzige -i examples/zitie.txt -o 练字帖.html --rows-per-char 2
tianzige --text "永和九年" --grid mi --repeat 10 --trace 3 -o 米字格.html
```

## clockdrill

[![CI](https://github.com/eastyou/clockdrill/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/clockdrill/actions/workflows/ci.yml)

钟表练习纸生成器：看钟面写时间、看时间画指针，或两者混合。钟面用 SVG 绘制，时针按分钟偏移，符合真实钟表；时间按 1/5/10/15/30 分钟间隔生成并自动去重。

```bash
clockdrill --mode mix --count 12 --granularity 15 -o 钟表练习.html
```

## wordsearch

[![CI](https://github.com/eastyou/wordsearch/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/wordsearch/actions/workflows/ci.yml)

英语单词找词游戏生成器：把单词表放进字母网格，横竖斜八个方向随机藏词，单词可交叉共用字母。输出可打印的游戏页和彩色高亮答案页，附起始行列与方向箭头。

```bash
wordsearch -i examples/words.txt -o 找词游戏.html --size 12
```

## graphpaper

[![CI](https://github.com/eastyou/graphpaper/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/graphpaper/actions/workflows/ci.yml)

方格纸、点阵纸、坐标纸生成器：选好类型和 2~20 毫米的间距，一条命令输出可直接打印的 A4 页面。坐标纸带居中的 x/y 轴、箭头、每格刻度和整厘米数字；每 10 毫米一条加深辅助线，数格子不费眼。

```bash
graphpaper --type coordinate --spacing 5 --title "函数图像练习" -o 坐标纸.html
graphpaper --type dot --spacing 10 --pages 2 -o 点阵纸.html
```

## nametag

[![CI](https://github.com/eastyou/nametag/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/nametag/actions/workflows/ci.yml)

姓名桌牌生成器：名单 CSV 两列「姓名,班级」，自动识别 UTF-8 与 GBK，生成 A4 折叠桌牌。上半张旋转 180°，沿虚线对折后前后两面都是正的；字号按姓名长度自适应，同班重名会列出所在行。

```bash
nametag -i examples/students.csv -o 姓名桌牌.html --columns 2 --rows 2
nametag -i 名单.csv --strict -o 桌牌.html
```

## maze

[![CI](https://github.com/eastyou/maze/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/maze/actions/workflows/ci.yml)

迷宫生成器：DFS 挖出没有环的完美迷宫，左上角入口、右下角出口，格子自动缩放到 A4 可用区域。加 `--solution` 追加答案页，用 BFS 求出最短通路并标注步数。

```bash
maze --width 15 --height 22 --seed 2026 --solution -o 迷宫.html
```

## sudoku

[![CI](https://github.com/eastyou/sudoku/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/sudoku/actions/workflows/ci.yml)

数独生成器：先生成完整解，再逐格挖洞，每挖一格都用回溯计数确认解仍然唯一。简单 40 个提示数、中等 33 个、困难 28 个，`--solution` 追加答案页，填入的数字用蓝色标出。

```bash
sudoku --difficulty medium --seed 2026 --solution -o 数独.html
```

## certkit

[![CI](https://github.com/eastyou/certkit/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/certkit/actions/workflows/ci.yml)

奖状生成器：用 Excel 维护一份「姓名,奖项,说明」名单，一条命令生成整套 A4 横向奖状。双线红框、红色「奖」印章、中文落款日期都是现成的，姓名过长自动缩小字号，正文自动折行。

```bash
certkit -i 获奖名单.csv --issuer 星海中学 --date 2026-11-21 -o 奖状.html
```

## readinglog

[![CI](https://github.com/eastyou/readinglog/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/readinglog/actions/workflows/ci.yml)

阅读记录表：把书单整理成「书名,作者,页数」，生成带序号、书名、作者、页数和开始/完成/签字栏的 A4 表格。按 `--rows` 自动分页，末页补空行，页脚统计总本数与总页数；不传书单则生成空白表。

```bash
readinglog -i 阅读书单.csv --rows 6 -o 阅读记录.html
```

## bingo

[![CI](https://github.com/eastyou/bingo/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/bingo/actions/workflows/ci.yml)

课堂宾果卡生成器：词表每行一个词，生成 A4 2×2 排版的卡片和末页三列叫号单。卡片互不重复，奇数尺寸中心留「★」自由格，支持 3×3、4×4、5×5 三种尺寸，`--seed` 固定后可以补印同一批。

```bash
bingo -i 单词表.csv --size 5 --count 8 --seed 2026 -o 宾果.html
bingo -i 单词表.csv --size 3 --count 30 --no-call-sheet -o 低年级宾果.html
```

## flashcard

[![CI](https://github.com/eastyou/flashcard/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/flashcard/actions/workflows/ci.yml)

双向记忆卡：读「术语,释义」CSV，每 4 张一组，先印正面再印同组背面。`--flip long` 长边翻页让背面左右镜像，`--flip short` 保持原序；释义自动折行并选择最大可用字号，`--no-back` 只印正面。

```bash
flashcard -i 记忆卡.csv -o 记忆卡.html
flashcard -i 记忆卡.csv --flip short --no-back -o 正面卡.html
```

## attendance

[![CI](https://github.com/eastyou/attendance/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/attendance/actions/workflows/ci.yml)

班级考勤表：名单生成整月 A4 横向表格，日列 1 到月末自动铺满，周末浅灰底、红色表头。超过每页行数自动分页并重复表头，日列按 267mm 可用宽度压缩，右侧留出勤、请假、迟到统计列。

```bash
attendance -i 名单.csv --month 2026-11 --rows 30 -o 考勤表.html
attendance -i 名单.csv --month 2026-11 --rows 15 --group 初二3班 -o 考勤表.html
```

---

## 开发约定

- 只依赖 Python 标准库，`pip install` 即可用
- 关键逻辑全部有单元测试，CI 覆盖 Python 3.9 ~ 3.13
- 输入校验与错误提示优先：文件不存在、编码错误、参数越界都会给出中文提示和明确退出码
- 提交信息遵循 Conventional Commits
