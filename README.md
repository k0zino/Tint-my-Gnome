# Tint my Gnome 51

Tints GNOME Shell 51 and libadwaita/GTK4 applications with the system accent
color.

This is an unofficial GNOME Shell 51 port of
[Tint my Gnome](https://github.com/pakovm-git/Tint-my-Gnome) by
[PakoVM](https://github.com/pakovm-git). All credit for the original design and
implementation goes to the original author.

## What it does

- Tints GNOME Shell 51 surfaces with 10% of the system accent color.
- Tints libadwaita / GTK4 applications through `~/.config/gtk-4.0/gtk.css`.
- Covers GNOME Shell 51 widgets, including the login dialog, parental controls,
  lock screen, workspace indicator and screenshot UI.
- Keeps dash icons transparent so Dash to Dock can draw its own highlight.
- Includes a settings page with a Flatpak override helper.

The accent color is controlled by **GNOME Settings → Appearance → Accent Color**.
There is no per-extension color setting.

## Install

```bash
gnome-extensions install --force tint-my-gnome-51@k0zino.shell-extension.zip
gnome-extensions enable tint-my-gnome-51@k0zino
```

Or copy this directory to:

```text
~/.local/share/gnome-shell/extensions/tint-my-gnome-51@k0zino/
```

## Flatpak applications

Open the extension settings and click **Apply GTK theme to Flatpaks**. This runs
`flatpak override` so Flatpak apps can read the GTK4 styling.

## Compatibility

- GNOME Shell 51.x
- GTK 4.24 / libadwaita 1.10
- Dark shell theme (the same limitation as the original extension)

## Donate

If you enjoy the original project, consider supporting its author:

⚡ Send some Bitcoin over Lightning to: pakovm@getalby.com
<img width="479" height="479" alt="lightning-address" src="https://github.com/user-attachments/assets/aa33e92c-36a3-43b7-b369-6a229a438f80" />

## License

GPL-3.0. See the upstream project for the original license.
