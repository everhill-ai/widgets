# EverHill widgets

**English** | [简体中文](README.zh-CN.md)

Put today's market drivers on your site: a free card with the day's most important market news
and the drivers behind it, written by [EverHill AI](https://everhill.ai/) and updated through
the day. English, Simplified Chinese and Traditional Chinese; light and dark.

Pick the options and copy the code at **https://everhill.ai/widgets/**, or paste this:

```html
<!-- EverHill widget -->
<div class="everhill-widget" data-widget="brief" data-lang="en" style="max-width:480px">
  <a href="https://everhill.ai/" target="_blank" rel="noopener" style="display:block;margin-top:6px;font:12px system-ui,sans-serif;color:#6b7280">Market news and drivers by EverHill AI</a>
</div>
<script async src="https://everhill.ai/widget.js"></script>
```

## Widgets

| Name    | `data-widget` | What it shows                                              | Example                              |
|---------|---------------|------------------------------------------------------------|--------------------------------------|
| Brief   | `brief`       | Today's most important market news and the drivers behind it | [brief/example.html](brief/example.html) |

## Options

| Attribute    | Values                         | Default                      |
|--------------|--------------------------------|------------------------------|
| `data-lang`  | `en`, `zh`, `zh-Hant`          | `en`                         |
| `data-theme` | `light`, `dark`                | the visitor's device setting |
| `data-ref`   | your EverHill referral code    | none                         |

- The card fills the width of its container; set `max-width` on the `div` to suit your page.
  Its height adjusts by itself.
- With `data-ref`, people who sign up from your widget count as your referrals. Your code is in
  the EverHill app under Account, Referral. Put the same code on the link:
  `https://everhill.ai/?ref=yourcode`.
- Adding a widget after the page has loaded (a single-page app)? Call
  `EverHillWidgets.mount()` once the `div` is in the page.

## How it works

`widget.js` puts a frame from everhill.ai above the link. The frame holds the card only: it sets
no cookies, asks for nothing and can't read your page.

## Questions

Open an [issue](../../issues) in this repository, or write to support@everhill.ai.

## Terms

The widget is free to use on the conditions in [LICENSE.md](LICENSE.md). In short:

- Free for any site, personal or commercial.
- The EverHill logo and the link to everhill.ai under the card must stay visible, unchanged
  and clickable.
- Show the card as it is: don't copy, alter or re-present its content.
- Information only, not investment advice. Provided as it is; it may change or be withdrawn.

© Evermountain International Pte. Ltd. EverHill™
