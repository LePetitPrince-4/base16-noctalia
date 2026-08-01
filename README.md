# base16-noctalia <img alt="Color wheel" src="https://raw.githubusercontent.com/tinted-theming/home/refs/heads/main/color_wheel.png" width="100" align="right" style="padding-top:0.6rem;">

This is a tinted-theming set for the [Noctalia desktop shell](https://github.com/noctalia-dev/noctalia)

## Basic Usage

download the theme you want and copy it into your `~/config/noctalia/palettes/` directory

then you can either

1. set the custom theme in the UI
2. run `$noctalia msg color-scheme-set custom base16-ayu-dark`
3. add the following to your [Noctalia settings](https://docs.noctalia.dev/v5/configuration/)

```toml
[theme]
custom_palette = "base16-ayu-dark"
source = "custom"
```

## Tinty Usage

first run `$ mkdir ~/.config/noctalia/palettes/`

Add the following toml settings to your [Tinty](https://github.com/tinted-theming/tinty) `~/.config/tinted-theming/tinty/config.toml` file:

```toml
[[items]]
path = "https://github.com/LePetitPrince-4/base16-noctalia"
name = "noctalia"
themes-dir = "palettes"
hook = "cp -f $TINTY_THEME_FILE_PATH ~/.config/noctalia/palettes/tinty.json && noctalia msg color-scheme-set custom tinty"
```

## Community

- [Tinted Theming Home](https://github.com/tinted-theming/home)
- Have something you want to discuss, but you're not sure it warrants an issue? Feel free to stop by
  [#tinted-theming:matrix.org](https://matrix.to/#/#tinted-theming:matrix.org) on [Matrix](https://matrix.org/).

## License

[MIT License](./LICENSE)
