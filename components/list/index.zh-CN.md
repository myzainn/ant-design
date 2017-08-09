---
category: Components
type: Data Display
title: List 
subtitle: 列表
cols: 1
---

通用列表。

## 何时使用

最基础的列表展示，可承载文字、列表、图片、段落，常用于后台数据展示页面。

## API

### List

| 参数     | 说明           | 类型     | 默认值       |
|----------|----------------|----------|--------------|
| bordered | 是否展示边框 | boolean   |  false  |
| loading | 当卡片内容还在加载中时，可以用 loading 展示一个占位 | boolean   |  false  |
| itemLayout | 设置 List.Item 布局, 设置成 vertical 则竖直样式显示, 默认横排 | string | - |
| showLoadMore    | 是否显示加载更多按钮 | boolean   |  false  |
| loadingMore  | 是否显示加载更多按钮的 loading 状态 | boolean   |  false  |
| onMoreClick    | 点击 more 按钮的回调 | function   | - |
| pagination | 对应的 pagination 配置, 设置 false 不显示 | boolean \| object   |  false  |

### List.Item

| 参数     | 说明           | 类型     | 默认值       |
---------|-------------|------|---------
| extra | 额外内容, 通常用在 itemLayout 为 vertical 的情况下, 展示右侧内容; horizontal 展示在列表元素最右侧 | string\|ReactNode |  -  |

### List.Item.Meta

| 参数     | 说明           | 类型     | 默认值       |
---------|-------------|------|---------
| avatar | 列表元素的图标 | ReactNode |  -  |
| title | 列表元素的标题 | string\|ReactNode |  -  |
| description | 列表元素的描述内容 | string\|ReactNode |  -  |

### List.Item.Action
| 参数     | 说明           | 类型     | 默认值       |
---------|-------------|------|---------
| actions | 如果此参数存在, 那么会将其中的数据转换成符合标准 ant design 设计的 action 样式元素 | Array |  -  |

### List.Item.Action actions props

| 参数     | 说明           | 类型     | 默认值          |
|----------|----------------|----------|-----------------|
| icon    | icon 图标           | string| -  |
| text      |  文案   |  string  | -               |
| onClick      | 点击回掉  |  function  | -  |