# 来源地图

这些是发现候选的入口，不是完整网站目录，也不是固定排名。先按技术栈、组件用途和想要的视觉方向选择少量来源，再打开具体组件及变体。允许用开放搜索发现新来源。

入口资料整理于 2026-10-30。网站名称、域名、产品边界、费用、许可证和可读性会变，使用时重新确认。不要把首页可打开当作某个具体组件已被查看。

## 有样式的组件与组合界面

| 来源与入口 | 优先查找 | 使用判断 |
| --- | --- | --- |
| [shadcn/ui](https://ui.shadcn.com/docs/components) | 基础控件、表单、数据展示、局部组合 | 检查具体变体和项目依赖，不假定所有版本使用同一底层库 |
| [coss ui](https://coss.com/ui) | 克制的表单控件、选择器、弹层 | Origin UI 旧入口当前重定向到此；沿实际页面确认产品和组件 |
| [Mantine](https://mantine.dev/) | React 表单、选择器、日期、上传、应用控件 | 适合探索完整应用中的控件状态；查看主题调整方式 |
| [HeroUI](https://heroui.com/) | React 控件、主题、选择器与组合 | 区分当前框架、产品及版本，具体风格以 Demo 为准 |
| [Material UI](https://mui.com/material-ui/) | Material 风格与应用控件 | 复杂表格、日期等产品能力和授权另查对应页面 |
| [Ant Design](https://ant.design/components/overview/) | 信息密集的表单、表格、筛选、反馈 | 默认样式可参考，项目中优先用现有主题体系协调 |
| [Element Plus](https://element-plus.org/en-US/component/overview.html) | Vue 表单、树、级联、表格、业务控件 | 适合查状态与组合，视觉定制成本仍需结合项目 |
| [Naive UI](https://www.naiveui.com/) | Vue 选择、树、数据与表单控件 | 页面依赖客户端渲染，文本读取为空时使用浏览器或换来源 |
| [PrimeVue](https://primevue.dev/) | Vue 数据控件、表单、菜单、排版组合 | 旧域名 primevue.org 当前重定向至此；查具体主题和产品边界 |
| [Nuxt UI](https://ui.nuxt.com/) | Vue / Nuxt 控件、表单、导航与组合 | 核对目标版本与框架支持；文本工具可能遇到 Markdown 内容协商 |
| [shadcn/vue](https://www.shadcn-vue.com/) | Vue 下的可定制控件与组合 | 不把 React API 和安装方式直接用于 Vue |
| [shadcn-svelte](https://www.shadcn-svelte.com/) | Svelte 下的控件与组合 | 确认目标 Svelte 版本；同款移植不作为额外设计方向 |
| [daisyUI](https://daisyui.com/components/) | Tailwind 控件、主题、轻量组合 | 样式与复杂交互需分开确认，不能仅凭 CSS 类承诺行为 |
| [Preline UI](https://preline.co/) | Tailwind 表单、导航、数据与 Blocks | 查看具体示例的 JavaScript、插件与依赖要求 |
| [Flowbite](https://flowbite.com/) | Tailwind 常规控件与组合 | 遇到抓取限制时换官方具体页面或浏览器，不把摘要当视觉证据 |
| [Tailwind Plus](https://tailwindcss.com/plus) | 应用局部组合、表单和布局 | 可能需要登录；只参考可见内容，不假定已获得代码访问权 |
| [PrimeNG](https://primeng.dev/) | Angular 表单、表格和业务组件 | 旧域名 primeng.org 当前重定向至此；以 Angular 版本为准 |
| [NG-ZORRO](https://ng.ant.design/) | Angular 的业务控件 | 可比较企业应用的密度和层级，不能复制 React 用法 |

## 个性样式、动效与真实产品参考

| 来源与入口 | 优先查找 | 使用判断 |
| --- | --- | --- |
| [Aceternity UI](https://ui.aceternity.com/) | 有辨识度的卡片、按钮、输入、动效和局部区块 | 宣传场景较多，应用控件仍以使用效率和状态完整度为先 |
| [Magic UI](https://magicui.design/) | 按钮、效果、动效、展示型局部组合 | 查看静态状态和实际依赖；不要默认用于密集表单 |
| [Motion Primitives](https://motion-primitives.com/) | 小尺度交互与动效细节 | 需要查看动态示例；抓取受限时按未确认处理 |
| [Uiverse](https://uiverse.io/) | 按钮、输入、开关、加载与单体视觉变体 | 指向作者具体作品，逐例核实代码形式和使用条件 |
| [Mobbin](https://mobbin.com/) | 真实产品中的组件组合与平台模式 | 主要作为视觉或流程参考；可能需要账号，不等于可复用组件代码 |
| [Page Flows](https://pageflows.com/) | 产品交互过程、局部状态和流程 | 可能限制抓取或访问；不可见的过程不描述成已看过 |

## 交互基础：用于适配判断，不直接充当皮肤

| 来源与入口 | 优先查找 | 使用判断 |
| --- | --- | --- |
| [Base UI](https://base-ui.com/) | React 选择、弹层、菜单等交互基础 | 无样式基础，需要具体示例或额外视觉方案 |
| [React Aria](https://react-aria.adobe.com/) | React 复杂选择、日期、国际化与交互 | 核对示例皮肤与行为文档，不将库的能力泛化到其他候选 |
| [Reka UI](https://reka-ui.com/) | Vue 可组合的交互原语 | 无样式基础；将具体 Example 和原语文档区分开 |
| [Bits UI](https://www.bits-ui.com/) | Svelte 交互基础 | 查具体示例，单独的 headless API 不构成视觉推荐 |

## 专门领域与移动端

| 来源与入口 | 优先查找 | 使用判断 |
| --- | --- | --- |
| [Ant Design Mobile](https://mobile.ant.design/) | 移动网页表单、弹层、列表和触屏模式 | 需要可见 Demo；桌面页面布局不代表移动效果 |
| [Vant](https://vant-ui.github.io/vant/) | Vue 移动网页控件、选择器和商品交互 | 查看移动预览，页面可能需要客户端渲染 |
| [AI Elements](https://ai-sdk.dev/elements/overview) | 聊天、输入区、来源和工具结果 | 核对当前组件与依赖；静态样式参考不要求接入模型服务 |
| [Prompt Kit](https://www.prompt-kit.com/) | 聊天输入、消息和 AI 局部组合 | 如无法打开 Demo，保留线索并找可确认的替代来源 |
| [Tiptap](https://tiptap.dev/) | 编辑器工具条、气泡菜单、内容输入组合 | 区分编辑器引擎、现成 UI 和可用扩展及其授权 |
| [FullCalendar](https://fullcalendar.io/) | 日历、排期、事件和时间视图 | 确认具体视图与功能；高级能力可能有独立授权 |
| [Apache ECharts](https://echarts.apache.org/) | 图表、图例、提示层与数据展示 | 用具体示例查看外观；不为选型生成无依据的业务数据 |
| [TanStack Table](https://tanstack.com/table/latest) | 数据表格行为与框架适配 | Headless 数据能力不等于现成表格皮肤，结合具体 styled example |

## 挑选路径

- **已有组件库的项目**：先找同库的变体、主题和组合；其他生态提供风格参考，不自动增加依赖。
- **未指定技术栈**：先比较视觉方向，候选标明代码生态；不默认所有人使用 React。
- **只有原生 HTML/CSS 的需求**：优先查提供相应示例的来源，确认交互是否需要脚本。
- **需要个性动效**：从动效来源补充一两个方向，与能融入页面的实用款比较。
- **复杂或新组件**：用领域词检索官方 Demo、作者实例、公开设计系统；这张表不限制来源。
- **原生应用或其他框架**：搜索该平台的官方组件或作者示例；网页组件仅在适合时作为视觉参考。

不要把网站自称的组件数量、宣传语、收费方案或性能指标写进推荐，除非当次需求需要且已核实。
