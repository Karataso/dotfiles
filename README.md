# A complete BSPWM Window Manager Environment
<div align = center>

![bspwm-dotfiles](https://github.com/gh0stzk/dotfiles/assets/67278339/0340846a-74d4-4a43-9430-142b0832738d)




&ensp;[<kbd> <br> Install <br> </kbd>](#-installation)&ensp;
&ensp;[<kbd> <br> Features <br> </kbd>](#-features)&ensp;
&ensp;[<kbd> <br> Themes <br> </kbd>](#-the-themes)&ensp;
&ensp;[<kbd> <br> Keybindings <br> </kbd>](#very-useful-keybindigs-to-know)&ensp;
&ensp;[<kbd> <br> Wiki <br> </kbd>](https://github.com/gh0stzk/dotfiles/wiki)&ensp;
<br><br><br></div>

https://github.com/user-attachments/assets/3eaae1e2-04dc-4a9b-8c91-139f85f5fb9e

<br>

## 👻 Welcome

Welcome to my dotfiles. I’m gh0stzk from Mexico.

These dotfiles are designed with the goal of providing a bspwm environment that is lightweight, efficient, and functional, tailored for any use—whether it’s gaming, web browsing, or a productive work setting.

You’ll have 12 unique themes to choose from, each with its own style, colors, and navigation bar options. With this variety, you’re sure to find one that suits your preferences and needs.

## :book: Wiki
I already started writing the [**Wiki**](https://github.com/gh0stzk/dotfiles/wiki), you should give it a read. If it is your first time with a WM, you may be interested in reading [First steps after installing the dotfiles](https://github.com/gh0stzk/dotfiles/wiki/Firsts-steps-after-installing) or maybe read [frequently asked questions and answers](https://github.com/gh0stzk/dotfiles/wiki/Questions---Answers) [Keybinds](https://github.com/gh0stzk/dotfiles/wiki/Keyboard-Shortcuts).

## 🚀 Features
<img src="https://user-images.githubusercontent.com/67278339/221605474-21d65156-0cf7-485c-bd1a-40792c37817e.png" alt="Linux Fetch" align="right" width="450">

#### Change themes on the fly

You can switch themes instantly, with no need to restart your session or environment. With just one click, the change is applied immediately.

#### Consistency Across the Environment

Unlike Matugen, Pywal, and other wallpaper-based theming tools, colors are not extracted from images. Every theme includes a handcrafted color palette, carefully selected to maintain consistency, readability, and visual appeal.

A modular theming system propagates these colors across the entire desktop environment. Switching themes instantly updates:

- BSPWM
- GTK (3.x)
- Dunst
- Rofi
- Kitty
- Eww
- Jgmenu
- Geany
- ScreenLocker (i3lock-color)
- Mpv Player
- Cava
- Zathura
- Polybar
- Cli-Tools
  - Yazi
  - Fzf-Tab
  - Bat
  - Eza
  - Ncmpcpp

Not all modules are enabled.

If you want to know how it works and how to enable or disable modules, go to [Color Modules](https://github.com/gh0stzk/dotfiles/wiki/Color-Modules)

ToDo-List:

- Obsidian
- Telegram-desktop
- Steam
- Btop
- Qt (5/6)
- Rmpc

#### Performance optimized

BSPWM is not a desktop environment (DE), and that’s exactly what makes it stand out in terms of lightweight performance. On my systems, my BSPWM-dotfiles environment starts with under **600 MB of RAM usage**. While these numbers don't tell the whole story, they do highlight the minimalist approach that a window manager should embrace.

In addition, each theme can be configured independently — either by manually editing the theme’s configuration file or using my RiceEditor application. This ensures a high level of customization: if you want a minimalist setup for a specific theme, you can disable animations, shadows, rounded borders, or fading effects. On the other hand, if you prefer a more visually rich theme with all those features enabled, that’s fully supported as well. My dotfiles are built to provide that level of flexibility.

#### Multi-Monitor support

If you have multiple monitors, BSPWM will automatically detect and configure up to 4 displays when launching with my dotfiles.

If you connect an additional monitor while the session is already running, simply reload BSPWM using the `Super + Alt + r` key combination, and your monitors will be configured instantly.

You can check the Wiki [👉 Monitors Setup](https://github.com/gh0stzk/dotfiles/wiki/Monitors-setup) if you want to edit the default layouts.

#### RiceEditor

Is an application designed to simplify the customization of your current theme. It allows you to easily adjust various visual and configuration aspects, tailoring your environment to your preferences without the need to manually edit configuration files.

#### Wallpaper Engines

My dotfiles support **5 different methods** for setting your favorite wallpaper:

1. **Random**: Sets a random wallpaper from the theme’s Walls directory.
2. **CustomDir**: Sets a random wallpaper from a directory you specify.
3. **Default**: Sets a specific image as wallpaper. (Default)
4. **CustomAnimated**: Supports animated wallpapers (.mp4, .mkv, .gif).
5. **Slideshow**: Changes the wallpaper every 15 minutes with a random image from the theme’s Walls directory.

Each option is **theme-specific**, meaning you can have an animated wallpaper in one theme, a static image in another, or a custom directory in a third — And all your settings will be preserved per theme. By default, all themes load a default wallpaper from their Walls Rice folder.

Check the wiki for more details: [👉 Wallpapers Configuration](https://github.com/gh0stzk/dotfiles/wiki/Wallpapers-Configuration)

#### Scratchpad

A _scratchpad_ is a tool designed to provide quick, temporary access to applications or notes without disrupting the desktop workflow. When activated, the scratchpad appears over the current workspace, allowing the user to access applications like a terminal, text editor, or any configured tool. Minimizing it hides the scratchpad from view but keeps it running in the background, ready to be reopened with a simple keyboard shortcut.

It's ideal for quick note-taking, running commands, or accessing auxiliary tools without losing focus on the current task.

#### Rofi Applets

Rofi applets to simplify your workflow:

- Wallpaper Selector - See the wiki [WallpaperSelector](https://github.com/gh0stzk/dotfiles/wiki/WallpaperSelector)
- Network Manager
- Bluetooth Controller
- Clipboard Manager
- Screenshot Tool
- Android MTP Manager
- Power Menu
- Keyboard Layout
- Rofi app launcher style selector
- Tab app switcher
- Pass Manager (Using pass app)

#### Optimized ZSH Configuration

Optimized, native ZSH configuration. Not __Oh-My-Zsh__ or other bloated plugin managers. Some features:

- Fastest and optimized performance compinit function
- Autocompletion
- Syntax highlighting
- History substring search
- Fzf-tab completion with previews!!

---

### 🎨 Launchers

| :tshirt: Theme Selector |
|:-:|
|![Screenshot-11_12_2023-01-06-03](https://github.com/gh0stzk/dotfiles/assets/67278339/b11b5c58-b9ec-446b-8980-4f77bebb3432)|

| :traffic_light: Wallpaper Selector |
|:-:|
|![Shot-2024-11-08-134530](https://github.com/user-attachments/assets/dbac8c47-f12c-4242-97d6-38ad1193f76b)|

| :tshirt: Bar Selector |
|:-:|
|![Bspwm Bar Selector](https://github.com/user-attachments/assets/94c4d699-890c-47d4-85dc-8e9622f4c679)|

### 🎨 The themes

| Nature | Dev |
|:-:|:-:|
| <img src="config/bspwm/rices/nature/preview.webp" alt="Nature rice"> | <img src="config/bspwm/rices/dev/preview.webp" alt="Dev rice"> |

| Cruel World | Sunset |
|:-:|:-:|
| <img src="config/bspwm/rices/cruel-world/preview.webp" alt="Cruel World rice"> | <img src="config/bspwm/rices/sunset/preview.webp" alt="Sunset rice"> |

| Grayscale | Silvia |
|:-:|:-:|
| <img src="config/bspwm/rices/grayscale/preview.webp" alt="Grayscale rice"> | <img src="config/bspwm/rices/silvia/preview.webp" alt="Silvia rice"> |

| Isabel | h4ck3r |
|:-:|:-:|
| <img src="config/bspwm/rices/isabel/preview.webp" alt="Isabel rice"> | <img src="config/bspwm/rices/h4ck3r/preview.webp" alt="h4ck3r rice"> |

---

### Rofi applets

| ![Shot-2024-11-09-131850](https://github.com/user-attachments/assets/05107f74-e137-41c0-9132-31d9c4fa0bb4) | ![Shot-2024-11-09-131918](https://github.com/user-attachments/assets/c5680b39-9aba-41e5-a781-7f23f7f8e336) |
| :--------------------------------------------------------------------------------------------------------: | :--------------------------------------------------------------------------------------------------------: |
|                                                 Power Menu                                                 |                                                Screenshoter                                                |

| ![Shot-2024-11-09-132031](https://github.com/user-attachments/assets/0893b0b6-1211-43cb-9923-f4e42af70f4b) | ![Shot-2024-11-09-133244](https://github.com/user-attachments/assets/03546cb9-cf0d-42a2-b424-458c887e67c2) |
| :--------------------------------------------------------------------------------------------------------: | :--------------------------------------------------------------------------------------------------------: |
|                                              Keyboard Layout                                               |                                               Android Mount                                                |

| ![Shot-2024-11-09-150142](https://github.com/user-attachments/assets/f7d1c404-c2e8-43c0-ad5e-6b052e3918c3) | ![Shot-2024-11-09-155335](https://github.com/user-attachments/assets/889d2ccf-beff-402d-8804-6d82c5638860) |
| :--------------------------------------------------------------------------------------------------------: | :--------------------------------------------------------------------------------------------------------: |
|                                              Network Manager                                               |                                             Clipboard Manager                                              |

| ![Shot-2024-11-09-153419](https://github.com/user-attachments/assets/4af56dfa-f61f-4b45-8350-d064fe67663a) | ![Shot-2024-11-09-153444](https://github.com/user-attachments/assets/fbd09603-8e8f-4cbb-a685-83a69a6d4c35) |
| :--------------------------------------------------------------------------------------------------------: | :--------------------------------------------------------------------------------------------------------: |
|                                             Bluetooth Manager                                              |                                              Terminal Manager                                              |

| ![Shot-2025-04-08-084756](https://github.com/user-attachments/assets/835366c8-88c5-4daf-8260-5c822e27abc8) | ![Shot-2025-04-08-084924](https://github.com/user-attachments/assets/c32f3cdb-7a5a-4372-b6f2-3f4a09f50868) |
| :--------------------------------------------------------------------------------------------------------: | :--------------------------------------------------------------------------------------------------------: |
|                                              Tab app switcher                                              |                                              Rofi style selector                                           |

| ![Shot-2025-04-08-084756](https://github.com/user-attachments/assets/59a84a0d-b471-444a-b4f9-091d4a0e51e2) |
| :--------------------------------------------------------------------------------------------------------: |
|                                              Rofi password manager                                         |

---

### Rofi app launcher styles
| ![Shot-2025-04-08-090012](https://github.com/user-attachments/assets/57ebcc98-73ea-4f76-bb2b-fe3f187be5e7) | ![Shot-2025-04-08-090041](https://github.com/user-attachments/assets/26361cd3-c3b4-48a2-a550-8df5cff120f5) | ![Shot-2025-04-08-090107](https://github.com/user-attachments/assets/16da6b0f-5a9e-4410-bb95-cb9fe696ce55) |
| :---: | :---: | :---: |
| Normal | Full | Minimal |

### Fzf tab terminal completions with previews!

| ![fzf tab](https://github.com/user-attachments/assets/2771e549-f7cc-44da-baf2-6c9fa299f0fb) |
| :---: |
| cd, ls, pacman, systemctl, kill, cat, commands with preview! |

### Eww widgets

| ![ProfilePane](https://github.com/user-attachments/assets/07827cff-63b9-40db-b0ef-8c214a5d8ec3) | ![MusicPlayer](https://github.com/user-attachments/assets/b96c49a1-57d1-43e5-bff0-cab2e6b4d101) |
| :---: | :---: |
| Profile Panel | Music Player |

---

### Rice Editor

| ![Shot-2024-11-09-155549](https://github.com/user-attachments/assets/2ac910c8-171f-47eb-8210-1469b6f75cc2) |
| :--------------------------------------------------------------------------------------------------------: |
|                                                Rice Editor                                                 |

### Lockscreen

| ![Lockscreen](https://github.com/user-attachments/assets/2f09b915-f426-49c3-b9b6-07be4e781f5a) |
| :--------------------------------------------------------------------------------------------: |
|                                           Lockscreen                                           |

### Jgmenu

| ![Jgmenu](https://github.com/user-attachments/assets/82daebec-66a6-4716-8e78-b02fcec7e77c) |
| :----------------------------------------------------------------------------------------: |
|                                           Jgmenu                                           |

## Yazi config

https://github.com/user-attachments/assets/8e15cc1a-88b8-4a7e-a4de-e7da76021406

## Scratchpad

https://github.com/user-attachments/assets/79764678-c519-4a41-a333-2a862a6d10f8

## Environment

| ![Gtk-Ranger-Music](https://github.com/user-attachments/assets/a7f7c082-5ffd-4a6c-babf-7361764cec80) |
| :--------------------------------------------------------------------------------------------------: |
|            The environment changes with each theme. In the gif: (Ranger, Thunar, Ncmpcpp)            |

## Very useful keybindigs to know...

Applications live on `ctrl` + `alt`, window and workspace management on `super`, session control on `super` + `alt`, and `alt` + key applies to the focused window.

| Keys | Action |
| :-------------------: | :---------------------------------------------------------------: |
| `ctrl` + `alt` + `t`<br>`ctrl` + `alt` + `shift` + `t` | Open a terminal<br>Open a floating terminal. |
| `alt` + `@space` | Apps menu. |
| `super` + `@space` | Theme (rice) selector. |
| `super` + `alt` + `@space` | Bar selector. |
| `ctrl` + `alt` + `w`<br>`ctrl` + `alt` + `e`<br>`ctrl` + `alt` + `f`<br>`ctrl` + `alt` + `m` | Browser<br>Editor<br>File manager<br>Music player |
| `ctrl` + `alt` + `s` | Takes a screenshot. |
| `ctrl` + `alt` + `p` | Power menu. |
| `ctrl` + `alt` + `l` | Lock the screen. |
| `super` + `w` | Opens a menu to select a wallpaper. |
| `super` + `alt` + `h`<br>`super` + `alt` + `u` | Hides bar/s<br>unhide bar/s |
| `alt` + `{plus,minus,0}` | Changes transparency on the focused window. |
| `alt` + `F4`<br>`alt` + `shift` + `F4` | Close the focused window<br>Force kill the focused window |
| `super` + `alt` + `r` | Restart bspwm. |
| `super` + `Escape` | Reload the keybinds. |
| `alt` + `F1` | Show the keybinds cheatsheet |

The cheatsheet is generated from `sxhkdrc`, so it always matches the bindings actually installed.

---

> [!CAUTION]
> ⚠️⚠️⚠️ My dotfiles are designed for a **1600x900** resolution with **96 DPI** on a single monitor.
> Some elements may appear different on higher or lower resolutions. You may need to make adjustments to adapt them to your preferences and setup. ⚠️⚠️⚠️

> [!important]
> ✏️✏️✏️ The installer assumes you already have a **functional** Arch Linux installation, whether it’s a fresh install or an existing setup.
>
> A login manager of your choice is required; **lightdm** is recommended.
>
> The rofi connection manager applet, works with **NetworkManager**
>
> If using a virtual machine, be sure to change the Picom backend from **glx** to **xrender** before rebooting, and verify that hardware acceleration is correctly configured in your VM. ✏️✏️✏️

> [!warning]
> :wrench::wrench::wrench: I have tested the installation and functionality of these dotfiles on both high- and low-end machines.
>
> Some adjustments may still be needed, such as changing the Picom backend or VSync settings to ensure compatibility with your graphics card.
>
> If you encounter any issues, feel free to open an [issue](https://github.com/gh0stzk/dotfiles/issues). :wrench::wrench::wrench:

---

### 💾 Installation:

> [!NOTE]
> The installer only works for **ARCH** Linux, and based distros. (Except NO-Systemd ditros like Artix)

Before running this command, check [RiceInstaller](https://raw.githubusercontent.com/Karataso/dotfiles/main/RiceInstaller) to make sure it's working and confirm it's safe for your system.

- Open a terminal and execute this commands one by one:

```sh
# Clone the dotfiles
git clone https://github.com/Karataso/dotfiles ~/dotfiles

# Run the installer from inside the clone
chmod +x ~/dotfiles/RiceInstaller
~/dotfiles/RiceInstaller
```

> [!NOTE]
> The installer installs straight from the clone it lives in. There is no second
download, so what ends up in `~/.config` is exactly the tree you cloned.
