# EverHill 小组件

[English](README.md) | **简体中文**

把今日市场驱动因素放到你的网站：一张免费的卡片，展示当天最重要的市场新闻及其背后的驱动因素，
由 [EverHill AI](https://everhill.ai/zh/) 撰写并全天更新。支持英文、简体中文和繁体中文，
以及浅色和深色。

在 **https://everhill.ai/zh/widgets/** 选好样式并复制代码，或直接粘贴下面这段：

```html
<!-- EverHill widget -->
<div class="everhill-widget" data-widget="brief" data-lang="zh" style="max-width:480px">
  <a href="https://everhill.ai/zh/" target="_blank" rel="noopener" style="display:block;margin-top:6px;font:12px system-ui,sans-serif;color:#6b7280">EverHill AI 提供的市场新闻与驱动因素</a>
</div>
<script async src="https://everhill.ai/widget.js"></script>
```

## 小组件

| 名称 | `data-widget` | 内容                                   | 示例                                     |
|------|---------------|----------------------------------------|------------------------------------------|
| 摘要 | `brief`       | 当天最重要的市场新闻及其背后的驱动因素 | [brief/example.html](brief/example.html) |

## 选项

| 属性         | 取值                  | 默认             |
|--------------|-----------------------|------------------|
| `data-lang`  | `en`、`zh`、`zh-Hant` | `en`             |
| `data-theme` | `light`、`dark`       | 跟随访客的设备   |
| `data-ref`   | 你的 EverHill 推荐码  | 无               |

- 卡片会占满所在容器的宽度；可在 `div` 上设置 `max-width`。高度会自动调整。
- 填入 `data-ref` 后，通过你的小组件注册的用户会计入你的推荐。推荐码在 EverHill 应用的
  「账户 → 推荐」中。链接上也请使用同一个推荐码：`https://everhill.ai/zh/?ref=你的推荐码`。
- 页面加载后才添加小组件（单页应用）？在 `div` 放入页面后调用一次 `EverHillWidgets.mount()`。

## 工作方式

`widget.js` 会在链接上方放入一个来自 everhill.ai 的框架。框架里只有卡片：不设置 Cookie，
不索取任何信息，也无法读取你的页面。

## 问题与反馈

请在本仓库提交 [issue](../../issues)，或发邮件至 support@everhill.ai。

## 使用条款

小组件可免费使用，条件见 [LICENSE.md](LICENSE.md)（以英文版为准）。简单来说：

- 任何网站都可免费使用，个人或商业均可。
- EverHill 标志和卡片下方指向 everhill.ai 的链接必须保持可见、未经改动、可以点击。
- 请按原样展示卡片：不要复制、改动内容，或当作自己的内容发布。
- 内容仅供参考，不构成投资建议。小组件按现状提供，可能调整或停止。

© Evermountain International Pte. Ltd. EverHill™
