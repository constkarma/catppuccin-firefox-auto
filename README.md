# Catppuccin Firefox Auto

A modern, adaptive Catppuccin theme for Firefox.

It uses **Catppuccin Latte** for light mode and **Catppuccin Frappé** for dark mode, with **Mauve** accents and automatic switching based on Firefox's light/dark color scheme.

> [!NOTE]
> This is an unofficial community project and is not an official Catppuccin port.

## Features

- Automatic light/dark switching
  - Light: Catppuccin Latte
  - Dark: Catppuccin Frappé
- Mauve accents
- Designed around modern Firefox UI
- Tuned for vertical tabs and the current sidebar layout
- Separate surface colors for:
  - browser chrome
  - URL bar
  - sidebar
  - Firefox Home / New Tab
- No JavaScript
- No content scripts
- No host permissions
- No data collection

The theme is implemented entirely with Firefox's static `theme` and `dark_theme` manifest entries.

## Design

This theme uses the Catppuccin palette while adapting its colors to the current Firefox interface rather than reproducing the older Catppuccin Firefox theme mapping exactly.

The main surface hierarchy is:

| Surface | Latte | Frappé |
| --- | --- | --- |
| Frame | Crust `#dce0e8` | Crust `#232634` |
| Toolbar | Mantle `#e6e9ef` | Mantle `#292c3c` |
| URL field | Base `#eff1f5` | Base `#303446` |
| Sidebar | Mantle `#e6e9ef` | Mantle `#292c3c` |
| New Tab background | Mantle `#e6e9ef` | Mantle `#292c3c` |
| New Tab cards | Base `#eff1f5` | Base `#303446` |
| Accent | Mauve `#8839ef` | Mauve `#ca9ee6` |

Structural separators use subtle, translucent Mauve accents. Solid Mauve is used for toolbar icons, popup borders, URL bar focus and text selection, tab activity, loading indicators, and attention states.

## Installation

### Temporary installation

1. Clone this repository, or download and extract its ZIP archive.
2. Open Firefox.
3. Navigate to `about:debugging`.
4. Select **This Firefox**.
5. Click **Load Temporary Add-on…**.
6. Select `manifest.json`.

The temporary installation remains active until Firefox is restarted.

### Permanent installation

Firefox requires add-ons and themes to be signed for normal permanent installation.

A packaged and signed release can be installed once one is provided through Mozilla Add-ons or another supported signed distribution method.

## Development

The theme is contained in `manifest.json` and does not require a build step.

After editing the manifest, reload the theme from:

`about:debugging` → **This Firefox** → **Reload**

## Privacy

This theme does not contain executable JavaScript and does not request access to webpages, tabs, browsing history, cookies, or other browsing data.

It does not make network requests or collect telemetry.

The light/dark transition is handled by Firefox itself through the static `theme` and `dark_theme` manifest entries.

## Acknowledgements

This project uses the [Catppuccin](https://github.com/catppuccin/catppuccin) color palette and was inspired by the earlier [Catppuccin Firefox](https://github.com/catppuccin/firefox) port.

Catppuccin is licensed under the MIT License.

Copyright © 2021 Catppuccin

This project is independently maintained and is not affiliated with or endorsed by the Catppuccin project or Mozilla.

## License

This project is licensed under the MIT License. See [`LICENSE`](./LICENSE).

Catppuccin-derived material remains subject to the Catppuccin MIT License and its original copyright notice. See [`LICENSES/Catppuccin.txt`](./LICENSES/Catppuccin.txt).
