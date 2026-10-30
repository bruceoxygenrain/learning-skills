# 组件与状态地图

按用户的组件定位相关行即可，不需要逐项阅读。覆盖范围开放：清单之外的组件用“触发器 + 内容容器 + 数据结构 + 交互行为”拆解，再检索同义词。

## 组件检索入口

| 类别 | 覆盖组件与常用英文检索词 | 重点观察 |
| --- | --- | --- |
| 按钮与操作 | button、icon button、button group、split button、toggle button、FAB、link、copy button、download button | 主次层级、图标与文字间距、忙碌态、禁用态、焦点 |
| 文本输入 | input、text field、textarea、search field、password、number input、OTP、PIN、input group、floating label、clearable input | 标签与提示位置、前后缀、聚焦、错误、长文本、密码显示 |
| 选值与搜索建议 | select、combobox、autocomplete、listbox、multi select、tag input、cascader、tree select、async select | 展开态、搜索、单多选、分组、长选项、空结果、已选项回显 |
| 布尔与分组选项 | checkbox、radio、switch、segmented control、toggle group、choice card、checkbox card | 开关与提交语义、选中对比、混合态、组标签、禁用 |
| 日期时间 | date picker、date range、calendar、time picker、datetime、month picker、year picker、wheel picker | 范围起止、禁用日期、快捷项、跨月、时区与本地格式 |
| 数值与颜色 | slider、range slider、stepper input、rating、color picker、color swatch、dial | 数值回显、刻度、拖动与键盘、触屏目标、颜色值 |
| 上传与文件 | file upload、dropzone、avatar upload、image crop、file list、attachment、upload queue | 拖放与点击、格式提示、进度、错误、重试、删除、缩略图 |
| 表单与校验 | form field、field group、inline form、dynamic form、multi step form、validation、field array | 标签对齐、必填提示、错误位置、分组、保存状态、步骤回退 |
| 导航 | navbar、sidebar、navigation rail、breadcrumb、tabs、bottom navigation、mega menu、pagination、command palette | 当前项、折叠、溢出、图标与层级、移动端收纳、键盘路径 |
| 菜单与浮层 | dropdown menu、context menu、popover、tooltip、hover card、nested menu | 触发方式、菜单分组、快捷键、嵌套、边界、关闭与焦点 |
| 对话框与面板 | dialog、modal、alert dialog、drawer、sheet、bottom sheet、side panel、confirmation | 标题与操作区、危险操作层级、内容滚动、尺寸、关闭方式 |
| 反馈与系统状态 | toast、notification、alert、banner、snackbar、progress、spinner、skeleton、empty state、error state、result | 反馈优先级、可恢复操作、时长、布局稳定、图标与文案 |
| 内容展示 | card、list item、badge、chip、tag、avatar、avatar group、stat、description list、accordion、timeline | 内容层次、密度、溢出、可点击范围、弱化信息、状态颜色 |
| 数据表格与树 | table、data grid、tree、tree table、virtual list、expandable row、row actions、column filter | 表头、行高、排序筛选、固定列、选择、批量操作、空与加载态 |
| 布局与工具区 | toolbar、filter bar、resizable panel、splitter、scroll area、sticky header、stack、divider、inspector panel | 对齐、间距、伸缩、滚动边界、窄屏收纳、操作优先级 |
| 图片与媒体 | carousel、image gallery、lightbox、image preview、video controls、audio player、thumbnail list | 主次图、裁切比例、翻页、缩放、控件可读性、触屏操作 |
| 编辑器与内容输入 | rich text editor、markdown editor、code editor、slash menu、bubble menu、mention、emoji picker | 选中态工具条、格式状态、长内容、浮层位置、保存与错误 |
| 聊天与 AI | chat bubble、message list、prompt input、composer、attachment、suggestion chip、model picker、citation、tool result、reasoning disclosure | 流式状态、停止与重试、附件、长代码、来源展开、历史会话 |
| 图表与数据概览 | chart、sparkline、KPI card、legend、chart tooltip、heatmap、gauge、map controls | 数据语义、单位、轴与图例、空数据、悬停、配色区分、可读性 |
| 工作流与排期 | kanban、drag handle、sortable list、calendar scheduler、stepper、activity feed、workflow node、Gantt | 拖动状态、落点、选中、状态变化、时间刻度、回退操作 |
| 账户与设置组合 | sign in form、account menu、organization switcher、theme toggle、language selector、settings section、permission matrix、billing selector | 当前身份、状态解释、字段分组、危险操作、保存反馈 |
| 商业与电商组合 | product card、pricing card、plan selector、quantity selector、cart item、address form、coupon input、checkout step、review card | 价格与单位、规格状态、优惠与校验、主操作、窄屏布局 |
| 移动与触屏模式 | action sheet、pull to refresh、swipe action、infinite scroll、bottom tab、mobile picker、mobile search、floating action | 点击目标、单手可达、手势提示、键盘遮挡、安全区、横竖屏 |

## 容易混淆的叫法

- **下拉框**：表单选值搜 Select；输入并搜索选项搜 Combobox / Autocomplete；执行操作搜 Dropdown Menu；命令入口搜 Command Palette。不能只因外观相近就替换语义。
- **标签**：切换内容搜 Tabs；描述状态搜 Badge / Tag；可删除选项搜 Chip / Token；字段标题搜 Label。
- **提示框**：简短悬停说明搜 Tooltip；可操作浮层搜 Popover；页面状态搜 Alert / Banner；短时消息搜 Toast；需要决策搜 Dialog。
- **步骤条与步进器**：流程进度搜 Stepper / Steps；数字加减搜 Number Input / Quantity Selector；结合上下文判断。
- **表格**：静态内容表和带排序、筛选、虚拟化的数据网格不同；仅样式需求不应引入复杂数据引擎。
- **抽屉与底部面板**：Drawer / Sheet / Bottom Sheet 的命名随库不同，结合方向、平台和交互查找。

## 用状态缩小搜索

按需要追加关键词：`open / expanded`、`focus`、`selected`、`disabled`、`loading`、`empty`、`error`、`multi-select`、`searchable`、`grouped`、`dense`、`dark`、`mobile`、`RTL`。

优先看会改变选款结论的状态。静态截图中看不到的交互写“未观察”，不从图上推断已实现。

## 清单外的组件

先描述它的用途，再拆解：例如“左侧可搜索树，右侧勾选结果”可以搜索 `tree transfer`、`dual listbox`、`multi select panel`，组合已有模式找局部参考。先查原生于该技术栈的实现，再找可借鉴视觉的其他生态；不要因为名称不在表中就结束任务。
