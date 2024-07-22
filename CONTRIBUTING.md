# Contributing

This repository includes a [GitHub Action] that builds the
colorschemes once a week. This keeps the colorschemes up-to-date
automatically.

## Building

### Dependencies

- `>=0.9.3` [tinted-builder-rust]

### Usage for template editing

1. Install [tinted-builder-rust]
1. `tinted-builder-rust build path/to/base16-hexchat`

### Usage for adding or editing a colorscheme

1. Clone the base16-hexchat
1. Clone [tinted-schemes]
1. Install [tinted-builder-rust]
1. Execute `tinted-builder-rust build base16-hexchat` with 
  - `--schemes-dir` arg - provide `/path/to/base16-scehemes`

```shell
tinted-builder-rust build /path/to/base16-hexchat \
  --schemes-dir /path/to/base16-schemes
```

If you have more questions about [tinted-builder-rust], have a look at
the information on the GitHub page.

[tinted-builder-rust]: https://github.com/tinted-theming/tinted-builder-rust
[tinted-schemes]: https://github.com/tinted-theming/schemes
[GitHub Action]: .github/workflows/update.yml
