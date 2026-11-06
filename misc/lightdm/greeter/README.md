# Greeter

A glassy LightDM login theme with a clock, user and session pickers, plus blur
and dim controls.

This is the [waifu-greeter](https://github.com/anime-kun32/waifu-greeter) theme by
[anime-kun32](https://github.com/anime-kun32), renamed to `greeter` and de-branded
for this dotfiles repo. The anime artwork was replaced with a wallpaper that isnt anime;
the layout and behaviour are theirs. Licensed GPL-3.0, see `LICENSE`.

## Requirements

- LightDM >= 1.19.0
- web-greeter >= 3.2.0 (AUR: `web-greeter`)

## Install

`RiceInstaller` installs this theme to `/usr/share/web-greeter/themes/greeter`
and points `/etc/lightdm/web-greeter.toml` at it.

Manually:

```bash
sudo mkdir -p /usr/share/web-greeter/themes
sudo cp -R greeter /usr/share/web-greeter/themes/
```

Then in `/etc/lightdm/web-greeter.toml`:

```toml
[greeter]
theme = "greeter"
```

## Changing the wallpaper

Replace `assets/bg.jpg` with your own image (1920x1080 or larger), or edit the
`background-image` rule in `css/style.css`.
