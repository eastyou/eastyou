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
| [answersheet](https://github.com/eastyou/answersheet) | 选择题答题卡：按题量生成 A4 涂卡答题卡 | 分栏分页、选项字母、打印排版 |
| [lessonplan](https://github.com/eastyou/lessonplan) | 教案模板：分节文本生成 A4 教案 | 文本解析、编码识别、文档排版 |
| [weeklyplan](https://github.com/eastyou/weeklyplan) | 学生周计划表：任务 CSV 生成一周计划 | 星期归一化、日期计算、打印排版 |
| [rubric](https://github.com/eastyou/rubric) | 评分量规：维度与等级 CSV 生成 A4 评价表 | CSV 校验、等级扩展、打印排版 |
| [syllabus](https://github.com/eastyou/syllabus) | 教学进度表：周次 CSV 生成学期进度表 | 周次校验、分页、打印排版 |
| [booklabel](https://github.com/eastyou/booklabel) | 图书标签：书名编号 CSV 生成标签纸 | 自动编号、行列布局、打印排版 |
| [homeworklog](https://github.com/eastyou/homeworklog) | 作业收缴表：学生名单与作业项目生成 A4 登记表 | 任务解析、连续编号、自动分页 |
| [parentlog](https://github.com/eastyou/parentlog) | 家校沟通记录：CSV 生成记录表，支持学生筛选与方式汇总 | 日期校验、精确筛选、统计分页 |
| [errorbook](https://github.com/eastyou/errorbook) | 错题整理册：错题 CSV 生成 A4 卡片与复习打卡页 | 科目筛选、卡片分页、打印排版 |
| [tangram](https://github.com/eastyou/tangram) | 七巧板活动包：精确裁剪图与拼搭挑战卡 | 多边形几何、面积守恒、SVG 排版 |
| [spirodraw](https://github.com/eastyou/spirodraw) | 万花尺描摹画册：参数方程生成内摆线画册 | 闭合周期、视觉去重、SVG 曲线 |
| [storydice](https://github.com/eastyou/storydice) | 故事骰子：四类故事要素的可打印折叠骰子 | 立方展开图、可复现随机、打印折叠 |
| [fractionkit](https://github.com/eastyou/fractionkit) | 分数条教具：精确等分的分数、小数、百分数对照条 | 分数运算、自适应字级、打印裁剪 |
| [numberline](https://github.com/eastyou/numberline) | 数轴练习纸：可配置范围、步长与留空标签 | 整数刻度、毫米排版、SVG |
| [geoboard](https://github.com/eastyou/geoboard) | 几何钉板：可打印点阵钉板与面积周长挑战卡 | 点阵坐标、题库、分页 |
| [metronome](https://github.com/eastyou/metronome) | 课堂节拍器：离线单文件，重拍高亮与倒计时 | Web Audio、状态机、响应式 |
| [morsecode](https://github.com/eastyou/morsecode) | 摩尔斯电码：命令行编解码与可打印练习卡 | 编码表、双向转换、打印排版 |
| [exitticket](https://github.com/eastyou/exitticket) | 课堂出门条：五种模板的 A4 四联反馈卡 | 模板注册表、裁切线、分页 |
| [starwheel](https://github.com/eastyou/starwheel) | 旋转星图：按纬度生成可裁剪组装的 A4 星图 | 极射投影、亮星星表、打印组装 |
| [moonphase](https://github.com/eastyou/moonphase) | 月相日历：月龄、月相图标与四相时刻 | 朔望周期、SVG 月相、日历排版 |
| [sundial](https://github.com/eastyou/sundial) | 日晷制作卡：按纬度计算时刻线的模板 | 日晷公式、半球镜像、模板排版 |
| [unitcircle](https://github.com/eastyou/unitcircle) | 单位圆转盘：三角函数值盘与对照表 | 弧度换算、三角函数、可剪指针 |
| [pixelgrid](https://github.com/eastyou/pixelgrid) | 像素画网格：坐标编号与按坐标涂色 | 行列坐标、图案缩放、颜色图例 |
| [storyboard](https://github.com/eastyou/storyboard) | 分镜纸：定格动画与短片分镜模板 | 分镜分页、画幅比例、通栏布局 |
| [cipherwheel](https://github.com/eastyou/cipherwheel) | 凯撒密码转盘：可打印同心圆盘、命令行编解码与解码练习卡 | 字母环旋转、SVG 同心圆、打印排版 |
| [logicgrid](https://github.com/eastyou/logicgrid) | 逻辑推理题生成器：4×4 逻辑网格，唯一解校验 | 排列枚举、线索贪心、唯一解 |
| [timeline](https://github.com/eastyou/timeline) | 历史事件时间轴：CSV 生成可打印的 A4 时间轴 | CSV 校验、比例定位、自动分页 |
| [mapgrid](https://github.com/eastyou/mapgrid) | 经纬网练习纸：可配置经纬范围、坐标题与答案页 | 等距投影、SVG 刻度、半球判断 |
| [quizbowl](https://github.com/eastyou/quizbowl) | 课堂抢答计分板：离线单文件、多队计分与倒计时 | 单文件 HTML、原生 JS、Web Audio |
| [patternblocks](https://github.com/eastyou/patternblocks) | 图案积木裁剪片：统一边长的几何积木与挑战卡 | 多边形几何、鞋带公式、页面布局 |
| [crossword](https://github.com/eastyou/crossword) | 填字游戏生成器：词条 CSV 自动交叉排版 | 交叉放置、网格编号、线索分类 |
| [nonogram](https://github.com/eastyou/nonogram) | 数织谜题：唯一解校验与行列提示 | 回溯求解、唯一性判定、网格分隔 |
| [poemcard](https://github.com/eastyou/poemcard) | 古诗竖排卡片：逐字排版的展示卡与书写稿纸 | 竖排布局、SVG 定位、自适应字号 |
| [cursive](https://github.com/eastyou/cursive) | 英文连笔字帖：四线三格描摹与空白练习行 | 四线格、按词换行、打印排版 |
| [slidingpuzzle](https://github.com/eastyou/slidingpuzzle) | 数字华容道：可解性判定、可打印棋盘与可玩版 | 逆序数、曼哈顿距离、单文件 HTML |
| [chessboard](https://github.com/eastyou/chessboard) | 国际象棋棋盘：FEN 局面、棋子裁剪片与练习卡 | FEN 解析、SVG 棋盘、Unicode 棋子 |
| [abacus](https://github.com/eastyou/abacus) | 算盘读数练习纸：数字画成上二下五的算盘 | 珠算模型、SVG 珠子、打印排版 |
| [spellingbee](https://github.com/eastyou/spellingbee) | 拼词蜂巢：7 字母谜题判词、计分与卡片 | 词表筛选、蜂巢几何、计分规则 |
| [truthtable](https://github.com/eastyou/truthtable) | 真值表工具：布尔表达式解析与练习纸 | 递归下降、运算符优先级、真值枚举 |
| [romannum](https://github.com/eastyou/romannum) | 罗马数字转换、标准写法校验与练习纸 | 减法记数、规范校验、题目生成 |
| [braille](https://github.com/eastyou/braille) | 英文盲文：Grade 1 编码解码与点字卡 | 六点单元、Unicode 盲文、点阵 SVG |
| [typingdrill](https://github.com/eastyou/typingdrill) | 离线英文打字练习：单文件 HTML | 实时高亮、WPM 统计、零依赖前端 |
| [numberbase](https://github.com/eastyou/numberbase) | 进制转换练习纸：2~36 进制互转与 A4 答案页 | 进制解析、随机出题、打印排版 |
| [cryptarithm](https://github.com/eastyou/cryptarithm) | 字母算式谜：求解与可打印练习纸 | 按列回溯、进位剪枝、唯一性校验 |
| [wordroots](https://github.com/eastyou/wordroots) | 英语词根词缀卡片与词义小测 | 词缀数据、干扰项生成、卡片排版 |
| [solarscale](https://github.com/eastyou/solarscale) | 太阳系比例海报：真实比例的天体与距离 | 比例换算、SVG 圆、A4 海报 |
| [staffnotes](https://github.com/eastyou/staffnotes) | 五线谱识谱卡：音名、频率与加线 | 谱表坐标、十二平均律、SVG 谱线 |
| [sentencemix](https://github.com/eastyou/sentencemix) | 句子重排练习纸：中英词卡打乱 | 分词、确定性打乱、打印排版 |
| [unitconv](https://github.com/eastyou/unitconv) | 单位换算练习纸：长度、质量、时间、容积 | 单位表、精确换算、打印排版 |
| [primefactor](https://github.com/eastyou/primefactor) | 质因数分解与因数树练习纸 | 试除分解、树布局、SVG 绘制 |
| [fractionops](https://github.com/eastyou/fractionops) | 分数四则运算练习纸与答案页 | Fraction、带分数解析、随机出题 |
| [noteduration](https://github.com/eastyou/noteduration) | 音符时值与小节补全练习 | 拍号换算、附点音符、SVG 符头 |
| [nets](https://github.com/eastyou/nets) | 长方体展开图：表面积、体积与折叠图 | 六面布局、尺寸校验、SVG 排版 |
| [symmetry](https://github.com/eastyou/symmetry) | 轴对称图形补全练习：四种对称轴 | 网格镜像、对称轴判定、打印排版 |
| [solarterms](https://github.com/eastyou/solarterms) | 二十四节气：太阳黄经推算日期、季节查询与年历练习纸 | 天文算法、日期推算、打印排版 |
| [idiomchain](https://github.com/eastyou/idiomchain) | 成语接龙：词库查询、接龙生成与练习纸 | 图搜索、回溯、打印排版 |
| [colorwheel](https://github.com/eastyou/colorwheel) | 色相环：互补、邻近、三角配色与练习纸 | HSL 换算、SVG 扇形、打印排版 |
| [rulerread](https://github.com/eastyou/rulerread) | 厘米尺读数：零刻度与非零起点练习纸 | SVG 刻度、长度换算、打印排版 |
| [change](https://github.com/eastyou/change) | 购物找零：总价、付款、找零与硬币图 | 整数分运算、贪心拆分、SVG |
| [venn](https://github.com/eastyou/venn) | 韦恩图：二/三集合交并差与练习纸 | 集合运算、区域枚举、SVG 三圆 |
| [protractor](https://github.com/eastyou/protractor) | 量角器：0–180° 内外圈读数与读角画角练习 | SVG 圆弧、角度分类、打印排版 |
| [thermometer](https://github.com/eastyou/thermometer) | 温度计：-30–50°C 读数与温差练习 | 刻度映射、零上零下、SVG |
| [numberbond](https://github.com/eastyou/numberbond) | 数的分合：十格阵与求部分求总数练习 | 分合模型、十格阵、打印排版 |
| [placevalue](https://github.com/eastyou/placevalue) | 位值积木：千/百/十/个读数与组数 | 数位拆解、积木绘制、打印排版 |
| [coordinate](https://github.com/eastyou/coordinate) | 四象限坐标：读点、连点成图与答案页 | 象限判定、坐标映射、SVG 网格 |
| [decimalgrid](https://github.com/eastyou/decimalgrid) | 小数方格图：涂色读数与小数百分数互化 | 百分位模型、约分、SVG 方格 |

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

## answersheet

[![CI](https://github.com/eastyou/answersheet/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/answersheet/actions/workflows/ci.yml)

选择题答题卡：给定题量与选项数，生成 A4 可打印答题卡。默认两栏、每栏 30 题，题目多了自动分页；选项圆圈从 A 到 F 自动编号，顶部留姓名、班级、学号、日期填写栏。

```bash
answersheet -q 50 --options 4 --columns 2 --subject 语文 -o 答题卡.html
answersheet -q 70 --options 2 --columns 1 -o 判断题答题卡.html
```

## lessonplan

[![CI](https://github.com/eastyou/lessonplan/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/lessonplan/actions/workflows/ci.yml)

教案排版工具：按「小节：」写纯文本，生成干净可打印的 A4 教案。科目、班级、课时自动排到页首，教学过程里的「导入：」不会误判成小节，`--teacher`、`--date` 可补执教与日期。

```bash
lessonplan -i 教案.txt --teacher 王老师 --date 2026-11-21 -o 教案.html
```

## weeklyplan

[![CI](https://github.com/eastyou/weeklyplan/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/weeklyplan/actions/workflows/ci.yml)

学生周计划表：读「星期,任务」CSV，生成一周七列、带勾选框的 A4 周计划。指定本周周一后，表头自动标出每一天的日期；不传任务文件就生成空白表，直接打印手写。

```bash
weeklyplan -i 任务.csv --start 2026-11-23 -o 周计划.html
weeklyplan --rows 6 -o 空白周计划.html
```

## rubric

[![CI](https://github.com/eastyou/rubric/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/rubric/actions/workflows/ci.yml)

评分量规：维度做行、等级做列，CSV 表头写等级名，一键生成 A4 横向评价表。支持 1~12 个维度、2~6 个等级，描述自动换行，学生自评、互评、教师评分都能直接在上面打勾。

```bash
rubric -i 作文量规.csv --task 写人作文 -o 评分量规.html
```

## syllabus

[![CI](https://github.com/eastyou/syllabus/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/syllabus/actions/workflows/ci.yml)

学期教学进度表：读「周次,日期,教学内容,作业」CSV，生成 A4 纵向进度表。周次自动校验、超出每页行数自动分页并重复表头，学期、学科、班级可组合成副标题。

```bash
syllabus -i 进度.csv --term 2026秋季学期 --subject 数学 --group 高一3班 -o 教学进度.html
```

## booklabel

[![CI](https://github.com/eastyou/booklabel/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/booklabel/actions/workflows/ci.yml)

班级图书角标签：读「书名,编号」CSV，生成 A4 标签纸。默认 3×8 共 24 个，虚线边框便于裁剪，书名按长度自动缩放，编号留空时自动补 `001`，底部可印归属文字。

```bash
booklabel -i 图书.csv --owner 三班图书角 -o 图书标签.html
booklabel -i 图书.csv --columns 2 --rows 6 -o 小标签.html
```

## homeworklog

[![CI](https://github.com/eastyou/homeworklog/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/homeworklog/actions/workflows/ci.yml)

班级作业收缴表：读单列学生名单，用 `--tasks` 指定要检查的作业，生成 A4 横向登记表。每页 20 人、序号跨页连续，预留手写作业格和备注栏，适合课前快速勾选。

```bash
homeworklog -i 学生.csv --tasks 语文练习册,数学口算,英语朗读 --date 2026-11-21 -o 作业收缴表.html
```

## parentlog

[![CI](https://github.com/eastyou/parentlog/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/parentlog/actions/workflows/ci.yml)

家校沟通记录表：读「日期,学生,方式,事项,后续」CSV，汇总沟通方式次数并生成 A4 记录表。支持按学生精确筛选，每页 12 条，长事项自动换行。

```bash
parentlog -i 沟通记录.csv --student 张三 -o 家校沟通记录.html
```

## errorbook

[![CI](https://github.com/eastyou/errorbook/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/errorbook/actions/workflows/ci.yml)

学生错题整理册：读「科目,题目,错因,正解,复习日期」CSV，生成两题一页的 A4 卡片。每题附三次复习打卡区，可按科目筛选，打印后就能装订使用。

```bash
errorbook -i 错题.csv --subject 数学 -o 数学错题册.html
```

## tangram

[![CI](https://github.com/eastyou/tangram/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/tangram/actions/workflows/ci.yml)

七巧板活动包：输出按真实毫米尺寸绘制的裁剪页与文字挑战卡。七块图块面积严格等于拼好的正方形，虚线裁剪、实线轮廓，每块标注名称和面积占比；挑战卡只给题目与提示，不泄露答案。

```bash
tangram --size 120 --copies 4 --challenges 4 -o 七巧板活动包.html
```

## spirodraw

[![CI](https://github.com/eastyou/spirodraw/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/spirodraw/actions/workflows/ci.yml)

万花尺描摹画册：用内摆线参数方程生成曲线，自动计算闭合圈数并挑选形状差异明显的参数组合。每条曲线附 R/r/d 参数表，最后一页说明如何用真实万花尺复现。

```bash
spirodraw --curves 6 --seed 42 -o 万花尺画册.html
```

## storydice

[![CI](https://github.com/eastyou/storydice/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/storydice/actions/workflows/ci.yml)

故事骰子：从内置角色、地点、冲突、转折四类词库生成可打印的十字展开图，带裁剪线、折线和粘贴边。剪下折好即可投掷，四颗骰子组合成一个故事开头，同一种子结果可复现。

```bash
storydice --sets 2 --seed 42 -o 故事骰子.html
```

## fractionkit

[![CI](https://github.com/eastyou/fractionkit/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/fractionkit/actions/workflows/ci.yml)

分数条教具：把 1 整条按分母 2~16 精确等分，每段同时标注分数、小数和百分数。用 `Fraction` 计算段宽，不产生浮点累积误差，虚线裁剪后可用于比大小、找等值分数。

```bash
fractionkit --max-denominator 12 --copies 2 -o 分数条教具.html
```

## numberline

[![CI](https://github.com/eastyou/numberline/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/numberline/actions/workflows/ci.yml)

数轴练习纸：设置起止范围、步长和留空规则，生成毫米级精度的 A4 数轴。零刻度加粗，被隐藏的数字只保留刻度线，适合读数、描点和不等式练习。

```bash
numberline --start -10 --end 10 --step 1 --blank-every 2 -o 数轴练习纸.html
```

## geoboard

[![CI](https://github.com/eastyou/geoboard/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/geoboard/actions/workflows/ci.yml)

几何钉板：输出 N×N 点阵钉板与面积、周长挑战卡。钉点坐标可测试，挑战题库 16 题，按种子洗牌，同一种子结果可复现。

```bash
geoboard --size 5 --boards 2 --challenges 4 -o 几何钉板.html
```

## metronome

[![CI](https://github.com/eastyou/metronome/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/metronome/actions/workflows/ci.yml)

课堂节拍器：单个离线 HTML，用 Web Audio 合成节拍声，重拍高亮，支持空格键启停、±5 BPM 调整、点击测速和练习倒计时，适合投影使用。

```bash
metronome --bpm 90 --beats 4 --accent 1 --minutes 5 -o 节拍器.html
```

## morsecode

[![CI](https://github.com/eastyou/morsecode/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/morsecode/actions/workflows/ci.yml)

摩尔斯电码工具：命令行双向编解码，支持字母、数字和常用标点；也能生成 A4 练习卡，正面写单词和书写线，答案单独成页。

```bash
morsecode --text "SOS 2026"
morsecode --decode "... --- ... / -.-"
morsecode --card --count 12 --seed 42 -o 摩尔斯练习卡.html
```

## exitticket

[![CI](https://github.com/eastyou/exitticket/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/exitticket/actions/workflows/ci.yml)

课堂出门条：内置 321 回顾、一句话总结、最困惑的地方、自评量表、快速检测五种模板。A4 每页 4 张，虚线裁剪，编号连续。

```bash
exitticket --template 321 --copies 4 -o 课堂出门条.html
```

## starwheel

[![CI](https://github.com/eastyou/starwheel/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/starwheel/actions/workflows/ci.yml)

旋转星图：内置 68 颗亮星，用极射赤面投影绘制星盘，再按纬度生成遮罩页。剪下两页、中心对齐、按月份和时刻转动，就能看到当夜星空；另附当夜可见亮星表。

```bash
starwheel --latitude 31.2 --month 3 --hour 21 -o 旋转星图.html
```

## moonphase

[![CI](https://github.com/eastyou/moonphase/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/moonphase/actions/workflows/ci.yml)

月相日历：计算整月每天月龄，用双圆遮挡绘制月相图标，标注新月与满月，并列出四个主要月相时刻（UTC）。适合天文课和自然观察记录。

```bash
moonphase --year 2026 --month 11 -o 月相日历.html
```

## sundial

[![CI](https://github.com/eastyou/sundial/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/sundial/actions/workflows/ci.yml)

日晷制作卡：按所在地纬度计算水平日晷的时刻线，输出晷面盘、晷针模板和校准说明三页。南纬会自动镜像，附各时刻线角度表。

```bash
sundial --latitude 31.2 -o 日晷制作卡.html
```

## unitcircle

[![CI](https://github.com/eastyou/unitcircle/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/unitcircle/actions/workflows/ci.yml)

单位圆转盘：把指定角度画在单位圆上，标注坐标、角度与弧度，附可剪指针、角度条和三角函数值表。90°与 270° 的 tan 显示「不存在」。

```bash
unitcircle --angles 0,30,45,60,90,120,135,150,180,210,225,240,270,300,315,330 -o 单位圆转盘.html
```

## pixelgrid

[![CI](https://github.com/eastyou/pixelgrid/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/pixelgrid/actions/workflows/ci.yml)

像素画网格：生成带 A~Z、AA… 列标与行号的坐标网格，附颜色编号示例和图例。学生按坐标涂色，同时练习坐标定位与颜色编码。

```bash
pixelgrid --width 16 --height 16 --pattern heart -o 像素画网格.html
```

## storyboard

[![CI](https://github.com/eastyou/storyboard/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/storyboard/actions/workflows/ci.yml)

分镜纸：为定格动画和短片准备的分镜模板，每格含 4:3 或 16:9 画面框、画面说明、台词音效和时长。奇数格时最后一格通栏，画面与填写区并排。

```bash
storyboard --frames 6 --per-page 3 --ratio 4:3 -o 分镜纸.html
```

## cipherwheel

[![CI](https://github.com/eastyou/cipherwheel/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/cipherwheel/actions/workflows/ci.yml)

凯撒密码转盘：一页 A4 打印出内外两圈字母，剪下内盘用图钉固定，旋转就能编解码。配套命令行编解码、26 种位移穷举，以及带答案页的解码练习卡。

```bash
cipherwheel disk -s 3 -o 转盘.html
cipherwheel encode "HELLO WORLD" -s 3
cipherwheel practice -n 10 -s 3 --answers -o 练习卡.html
```

## logicgrid

[![CI](https://github.com/eastyou/logicgrid/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/logicgrid/actions/workflows/ci.yml)

4×4 逻辑推理题生成器：4 个人、4 种颜色、4 种宠物、4 个地点，随机出题后穷举 13824 种组合校验唯一解，输出 A4 题面（打勾网格 + 线索列表）与答案页。

```bash
logicgrid --seed 7 --count 2 -o 推理题.html
```

## timeline

[![CI](https://github.com/eastyou/timeline/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/timeline/actions/workflows/ci.yml)

事件 CSV 一行一件事，表头为 `year,title,description,category`。按年份排序、按比例在年代尺上定位、自动分页，并可按分类与年份区间筛选，输出可打印的时间轴。

```bash
timeline demo -o events.csv
timeline -i events.csv --start 1900 --end 2000 --category 科技 -o 时间轴.html
```

## mapgrid

[![CI](https://github.com/eastyou/mapgrid/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/mapgrid/actions/workflows/ci.yml)

经纬网练习纸：可配置经纬范围与刻度间隔，生成四边带刻度的 SVG 网格，自动配「给坐标找位置」和「看图写坐标」两类题，附答案页与半球判断。

```bash
mapgrid -o 经纬网.html --lat-min -60 --lat-max 60 --step 15 --questions 8
```

## quizbowl

[![CI](https://github.com/eastyou/quizbowl/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/quizbowl/actions/workflows/ci.yml)

课堂抢答计分板：生成一个不引用任何网络资源的单文件 HTML，双击即用。每队一张卡片，键盘 A/S/D/F 给对应队伍加分，空格键控制倒计时，Z 撤销，R 重置，可全屏投影。

```bash
quizbowl -o 计分板.html --teams "红队,蓝队,黄队,绿队" --seconds 60
```

## patternblocks

[![CI](https://github.com/eastyou/patternblocks/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/patternblocks/actions/workflows/ci.yml)

图案积木裁剪片：等边三角形、菱形、梯形、正六边形、正方形统一使用 30mm 边长，三角形族面积比严格为 1:2:3:6。输出多页 A4 裁剪图、面积对照表与拼图挑战卡。

```bash
patternblocks -o 积木.html --side 30 --each 6
```

## crossword

[![CI](https://github.com/eastyou/crossword/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/crossword/actions/workflows/ci.yml)

读入「词条,线索」CSV，自动寻找共享字符把词语交叉排进网格，生成带编号的 A4 填字题、横向与纵向线索列表，并附答案页。

```bash
crossword demo -o words.csv
crossword -i words.csv --size 13 --seed 3 -o 填字.html
```

## nonogram

[![CI](https://github.com/eastyou/nonogram/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/nonogram/actions/workflows/ci.yml)

随机生成黑白格图案，计算行列提示数，并用回溯求解器校验唯一解，输出 A4 数织题面与答案页。

```bash
nonogram --size 10 --seed 5 -o 数织.html
```

## poemcard

[![CI](https://github.com/eastyou/poemcard/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/poemcard/actions/workflows/ci.yml)

内置 12 首公版古诗，把诗句逐字排成竖排（自上而下、自右向左）的 A4 展示卡，逐字 SVG 定位，不依赖 CSS 竖排特性，另可输出稿纸格与临写页。

```bash
poemcard --all -o 古诗卡.html
poemcard --poem 静夜思 --grid -o 稿纸.html
```

## cursive

[![CI](https://github.com/eastyou/cursive/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/cursive/actions/workflows/ci.yml)

把单词或句子排成标准四线三格：上伸线、虚线中线、基线、下伸线；支持全描摹、两行描摹其余留白、全空白三种模式。

```bash
cursive --text "The quick brown fox jumps over the lazy dog." --style fade -o 字帖.html
cursive --alphabet -o 字母.html
```

## slidingpuzzle

[![CI](https://github.com/eastyou/slidingpuzzle/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/slidingpuzzle/actions/workflows/ci.yml)

3×3 / 4×4 数字华容道：用逆序数判定可解性，洗牌保证一定可还原；可打印棋盘与编号方块，也能生成离线可玩的单文件 HTML。

```bash
slidingpuzzle --size 3 --seed 9 -o 华容道.html --playable
```

## chessboard

[![CI](https://github.com/eastyou/chessboard/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/chessboard/actions/workflows/ci.yml)

把 FEN 局面渲染成 A4 棋盘，带 a-h / 1-8 坐标与棋子字形；另附 24 枚棋子裁剪片和走法练习卡。

```bash
chessboard -o 棋盘.html
chessboard --fen "8/8/8/4k3/8/8/4K3/8 w - - 0 1" -o 残局.html
```

## abacus

[![CI](https://github.com/eastyou/abacus/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/abacus/actions/workflows/ci.yml)

上二下五的中式算盘：每根档位 2 颗上珠、5 颗下珠，靠梁计数。把任意数字画成算盘，或一次生成整页读数练习，答案页可选。

```bash
abacus svg 3806 --rods 4 --digits -o 3806.svg
abacus sheet -o 练习.html --count 12 --digits 4 --seed 2026 --answers
```

## spellingbee

[![CI](https://github.com/eastyou/spellingbee/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/spellingbee/actions/workflows/ci.yml)

七字母拼词蜂巢：中心字母必须使用，单词至少 4 个字母。从词表一次求出全部合法词并按规则计分，全字母词额外加 7 分；卡片带蜂巢、书写行与答案页。

```bash
spellingbee solve --letters abcdefg --center a --words words.txt
spellingbee card --letters abcdefg --center a --words words.txt --answers -o 卡片.html
```

## truthtable

[![CI](https://github.com/eastyou/truthtable/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/truthtable/actions/workflows/ci.yml)

布尔表达式递归下降解析，支持 `not` / `and` / `or` / `xor` / `->` / `<->` 及常见符号写法。枚举真值表、判断重言式与矛盾式，并生成留空待填的 A4 练习纸。

```bash
truthtable eval "A and (B or not C)"
truthtable info "A or not A"
truthtable sheet examples/expressions.txt --answers -o 练习.html
```

## romannum

[![CI](https://github.com/eastyou/romannum/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/romannum/actions/workflows/ci.yml)

1~3999 双向转换，并严格校验标准写法：`IIII`、`VX`、`IL` 等会被拒绝。练习纸支持「数字→罗马数字」「罗马数字→数字」与混合模式，附常用对照表。

```bash
romannum to 1997
romannum from mcmxcvii
romannum sheet --max 1000 --mode to-roman --answers -o 练习.html
```

## braille

[![CI](https://github.com/eastyou/braille/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/braille/actions/workflows/ci.yml)

英文一级盲文：26 个字母、数字号、大写号与常用标点双向转换；点阵 SVG 可打印，支持「读盲文写单词」与「看单词点写盲文」两种卡片，另附字母对照表。

```bash
braille encode "Hello"
braille decode "⠓⠑⠇⠇⠕"
braille card words.txt --mode read --answers -o 点字卡.html
braille chart -o 字母表.html
```

## typingdrill

[![CI](https://github.com/eastyou/typingdrill/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/typingdrill/actions/workflows/ci.yml)

六套内置课程（基准键、上排键、下排键、数字、句子、代码），也支持自定义文本。生成单文件 HTML，逐字符高亮、实时 WPM 与正确率、限时结算，完全离线。

```bash
typingdrill lessons
typingdrill build --lesson home --minutes 3 -o 打字练习.html
typingdrill build --text examples/custom.txt -o 自定义.html
```

## numberbase

[![CI](https://github.com/eastyou/numberbase/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/numberbase/actions/workflows/ci.yml)

二进制、八进制、十进制、十六进制之间的互转练习：支持 2~36 任意进制，同页题目不重复，`--answers` 生成独立答案页。解析会指出具体是哪个字符不合法。

```bash
numberbase convert 255 --to 16
numberbase convert ff --from 16 --to 2
numberbase sheet --count 20 --from 10 --to 2 --seed 7 --answers -o worksheet.html
```

## cryptarithm

[![CI](https://github.com/eastyou/cryptarithm/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/cryptarithm/actions/workflows/ci.yml)

字母算式谜：相同字母代表相同数字，不同字母代表不同数字。按列从右向左回溯并剪掉不可能的进位，常见题目毫秒级出解；内置 6 道经典题，可生成练习纸与答案页。

```bash
cryptarithm solve "SEND + MORE = MONEY"
cryptarithm solve "TWO + TWO = FOUR" --all
cryptarithm sheet --count 4 --seed 3 --answers -o puzzles.html
```

## wordroots

[![CI](https://github.com/eastyou/wordroots/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/wordroots/actions/workflows/ci.yml)

36 条常用前缀、词根与后缀，支持按词条、释义、例词搜索；可生成两栏 A4 卡片，或带干扰项的词义小测。干扰项优先取自同一类型，答案页单独分页。

```bash
wordroots list --kind prefix
wordroots find tele
wordroots cards --count 12 --seed 3 -o cards.html
wordroots quiz --count 10 --seed 3 --answers -o quiz.html
```

## solarscale

[![CI](https://github.com/eastyou/solarscale/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/solarscale/actions/workflows/ci.yml)

太阳与八大行星按真实比例画成圆，同时换算「如果距离也按同一比例摆放，需要多长的纸」。按 1 毫米 = 8000 千米，太阳能装进 A4，而海王星要放到 560 米外。

```bash
solarscale poster --km-per-mm 8000 -o poster.html
solarscale poster --fit Sun --width 180 -o sun.html
solarscale table --km-per-mm 8000
solarscale info Earth
```

## staffnotes

[![CI](https://github.com/eastyou/staffnotes/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/staffnotes/actions/workflows/ci.yml)

随机抽取音名画成五线谱，生成 A4 识谱卡。支持高低音谱号、自定义音域、加线计算与十二平均律频率，答案可单独打印。

```bash
staffnotes sheet --count 8 --clef treble --seed 3 --answers -o sheet.html
staffnotes list --clef bass
staffnotes note C4
```

## sentencemix

[![CI](https://github.com/eastyou/sentencemix/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/sentencemix/actions/workflows/ci.yml)

把英文单词或中文汉字打乱成词卡，生成语序练习纸。打乱结果一定与原句不同，同一个种子可复现；支持文本文件一行一句，自动跳过空行与注释。

```bash
sentencemix sheet --count 6 --seed 3 --answers -o sheet.html
sentencemix sheet -i sentences.txt --answers
sentencemix mix "The cat sleeps on the sofa." --seed 1
```

## unitconv

[![CI](https://github.com/eastyou/unitconv/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/unitconv/actions/workflows/ci.yml)

长度、质量、时间、容积四类单位的换算工具，既能查单个数值，也能一次生成整页 A4 换算练习。答案带单位，种子固定时题目可复现。

```bash
unitconv convert 3.5 --from km --to m
unitconv units --category mass
unitconv sheet --category length --count 20 --seed 7 --answers -o sheet.html
```

## primefactor

[![CI](https://github.com/eastyou/primefactor/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/primefactor/actions/workflows/ci.yml)

质数判定、质因数分解、全部因数与因数树一步到位。练习纸随机抽题，答案页把分解过程画成树，适合讲“短除法”与“分解质因数”。

```bash
primefactor factorize 360
primefactor divisors 360
primefactor sheet --count 8 --seed 5 --answers -o sheet.html
```

## fractionops

[![CI](https://github.com/eastyou/fractionops/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/fractionops/actions/workflows/ci.yml)

用标准库 `fractions.Fraction` 做分数四则运算，支持 `3/4`、`1 1/2`、`-1 1/2` 等写法。可只出加减或四则混合，答案自动约分并转成带分数。

```bash
fractionops calc "1 1/2" + "3/4"
fractionops sheet --count 20 --ops +,- --seed 5 --answers -o sheet.html
fractionops sheet --count 12 --ops +,-,*,/ --negative -o mixed.html
```

## noteduration

[![CI](https://github.com/eastyou/noteduration/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/noteduration/actions/workflows/ci.yml)

从全音符到十六分音符，附点自动乘 1.5，拍号统一换算成四分音符拍数。题目给出不完整小节，问“还差几拍”，答案支持整数与分数。

```bash
noteduration notes
noteduration note "dotted half"
noteduration sheet --signature 6/8 --count 8 --seed 3 --answers -o sheet.html
```

## nets

[![CI](https://github.com/eastyou/nets/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/nets/actions/workflows/ci.yml)

把长方体和正方体画成标准十字展开图，每个面标注名称与边长，沿实线裁剪、沿相邻边折叠即可成型。同时给出表面积、体积与展开图尺寸。

```bash
nets net 5 4 3 -o cuboid.html
nets info 5 4 3
nets sheet --count 8 --seed 3 --answers -o sheet.html
```

## symmetry

[![CI](https://github.com/eastyou/symmetry/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/symmetry/actions/workflows/ci.yml)

在方格纸上补全轴对称图形。支持竖直、水平、主对角线、副对角线四种对称轴，答案用浅黄色标出需要补的格子，也可以直接查询任意格点图形的对称轴。

```bash
symmetry axes "0,0 0,2 1,1" --size 3
symmetry complete "0,0" --size 4 --axis vertical
symmetry sheet --count 8 --seed 3 --answers -o sheet.html
```

## solarterms

[![CI](https://github.com/eastyou/solarterms/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/solarterms/actions/workflows/ci.yml)

按太阳视黄经每 15° 推算二十四节气日期，支持 1900–2100 年。可查询季节、下一个节气与两个节气之间的天数，并生成四季节气年历和带答案的练习纸。

```bash
solarterms year 2026
solarterms term 2026 立春 --to 春分
solarterms calendar --year 2026 -o calendar.html
solarterms sheet --count 12 --seed 3 --answers -o sheet.html
```

## idiomchain

[![CI](https://github.com/eastyou/idiomchain/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/idiomchain/actions/workflows/ci.yml)

内置 224 条常用成语与释义，按首尾字接龙。可从任意成语随机生成 2–8 个成语的接龙，校验首尾相接与重复，按首字查词，并生成带答案的 A4 练习纸。

```bash
idiomchain chain 一心一意 --length 5 --seed 7
idiomchain info 一心一意
idiomchain find 一 --limit 10
idiomchain sheet --count 12 --seed 3 --answers -o sheet.html
```

## colorwheel

[![CI](https://github.com/eastyou/colorwheel/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/colorwheel/actions/workflows/ci.yml)

12 色与 24 色两套色相环，红色在正上方顺时针排列。自动计算互补色、邻近色与三角配色，生成含 SVG 色环与配色关系表的页面，以及认色、互补、邻近、三角四类练习纸。

```bash
colorwheel wheel --size 24 -o wheel.html
colorwheel color 红
colorwheel sheet --count 12 --seed 3 --answers -o sheet.html
```

## rulerread

[![CI](https://github.com/eastyou/rulerread/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/rulerread/actions/workflows/ci.yml)

按真实比例画出 0–10 厘米刻度尺，用色块标出物体，练习零刻度与非零起点两种读数。答案统一换算成毫米比较，支持厘米、毫米、厘米 + 毫米多种写法。

```bash
rulerread length 2.5 7.5
rulerread length 2 9 --svg
rulerread sheet --count 12 --seed 3 --answers -o sheet.html
```

## change

[![CI](https://github.com/eastyou/change/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/change/actions/workflows/ci.yml)

20 件文具商品的购物找零题，金额以整数分存储。付款从 5/10/20/50/100 元中选取，找零自动拆成纸币与硬币，答案页附 SVG 示意图。

```bash
change change 12.5 20
change catalog
change sheet --count 12 --seed 3 --answers -o sheet.html
```

## venn

[![CI](https://github.com/eastyou/venn/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/venn/actions/workflows/ci.yml)

全集 1–30，内置倍数、大小比较、个位数字等 8 条集合规则。支持 2 圆与 3 圆韦恩图，生成只在集合中、交集、并集、差集四类题目，答案按集合比较且顺序无关。

```bash
venn rules
venn sheet --count 12 --size 3 --seed 3 --answers -o sheet.html
venn sheet --count 10 --size 2 --kinds union,difference -o two-sets.html
```

## protractor

[![CI](https://github.com/eastyou/protractor/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/protractor/actions/workflows/ci.yml)

半圆量角器 SVG，1°/5°/10° 三级刻度与内外双圈读数。读角题自动画出角终边，画角题只给空白量角器，支持锐角、直角、钝角分类与随机种子复现。

```bash
protractor sheet --count 8 --answers -o sheet.html
protractor sheet --kinds read --min 30 --max 150 -o read.html
protractor classify 120
```

## thermometer

[![CI](https://github.com/eastyou/thermometer/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/thermometer/actions/workflows/ci.yml)

-30–50°C 竖直温度计，水银柱随温度升降。读数题看温度计写数，温差题计算从零下到零上的变化，自动判断上升或下降。

```bash
thermometer sheet --count 8 --answers -o sheet.html
thermometer show 15 -o temp.svg
thermometer diff -4 6
```

## numberbond

[![CI](https://github.com/eastyou/numberbond/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/numberbond/actions/workflows/ci.yml)

三圆分合图加 2×5 十格阵，空缺位置可选总数、左边或右边。总数不超过 10 时自动附上圆点图，帮助理解整体与部分的关系。

```bash
numberbond sheet --count 8 --answers -o sheet.html
numberbond sheet --missing left,right --min 5 --max 10 -o part.html
numberbond bond 10 --left 3 --missing whole -o bond.svg
```

## placevalue

[![CI](https://github.com/eastyou/placevalue/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/placevalue/actions/workflows/ci.yml)

把四位数画成千位立方体、百位 10×10 平板、十位长条和个位小方块。看积木写数、按数说积木两种题型，另附数位拆解与合成命令。

```bash
placevalue sheet --count 8 --answers -o sheet.html
placevalue blocks 3205 -o blocks.svg
placevalue split 3205
```

## coordinate

[![CI](https://github.com/eastyou/coordinate/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/coordinate/actions/workflows/ci.yml)

-10–10 四象限坐标系，1 格 1 单位。读点题自动标注字母，连点题给出坐标清单，内置房子、小鱼、五角星三种图形，答案页附连线结果。

```bash
coordinate sheet --count 8 --answers -o sheet.html
coordinate grid -o grid.svg
coordinate where -3 4
```

## decimalgrid

[![CI](https://github.com/eastyou/decimalgrid/actions/workflows/ci.yml/badge.svg)](https://github.com/eastyou/decimalgrid/actions/workflows/ci.yml)

10×10 方格图当作“1”，涂色格数就是百分位。支持涂色读数、按小数涂色、小数与百分数和最简分数互化，百分数转分数自动约分。

```bash
decimalgrid sheet --count 8 --answers -o sheet.html
decimalgrid grid 37 -o grid.svg
decimalgrid convert 0.75
```

---

## 开发约定

- 只依赖 Python 标准库，`pip install` 即可用
- 关键逻辑全部有单元测试，CI 覆盖 Python 3.9 ~ 3.13
- 输入校验与错误提示优先：文件不存在、编码错误、参数越界都会给出中文提示和明确退出码
- 提交信息遵循 Conventional Commits
