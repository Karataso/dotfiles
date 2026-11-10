# Greeter (optional web-greeter theme)

A glassy LightDM login theme with a clock, user and session pickers, plus blur
and dim controls.

This is the [waifu-greeter](https://github.com/anime-kun32/waifu-greeter) theme by
[anime-kun32](https://github.com/anime-kun32), renamed to `greeter` and de-branded
for this dotfiles repo. The anime artwork was replaced with a wallpaper that is not
anime; the layout and behaviour are theirs. Licensed GPL-3.0, see `LICENSE`.

## Not installed by default

The installer uses **`lightdm-gtk-greeter`** and themes it from the active rice at
every boot through `/usr/local/bin/dots-greeter`: that script gives the greeter the
rice's GTK, icon and cursor themes and picks a random wallpaper from its `walls/`
directory. Nothing needs web-greeter for that.

`web-greeter` lives in the AUR, is slow to build and, with `detect_theme_errors`
on, quietly swaps in a stock theme when a custom one throws — which is why it is
only used when it is already installed, and why this theme is **kept for reference,
not deployed**. The installer never copies it anywhere.

## Installing it yourself

If you do want it, install `web-greeter` and copy the theme:

```bash
sudo mkdir -p /usr/share/web-greeter/themes
sudo cp -R misc/lightdm/greeter /usr/share/web-greeter/themes/greeter
```

Then in `/etc/lightdm/web-greeter.toml`:

```toml
[greeter]
theme = "greeter"
```

and in `/etc/lightdm/lightdm.conf`, under `[Seat:*]`:

```ini
greeter-session=web-greeter
```

`dots-greeter` only repaints a web-greeter theme whose `index.html` links
`dots-wallpaper.css` (the installer adds that link when it configures the theme).
This theme does not include it, so installed by hand it keeps its own background
(`assets/bg.jpg`). Add `<link rel="stylesheet" href="dots-wallpaper.css">` to
`index.html` if you want it to follow the active rice instead.

## Changing the wallpaper

Replace `assets/bg.jpg` with your own image (1920x1080 or larger), or edit the
`background-image` rule in `css/style.css`.
