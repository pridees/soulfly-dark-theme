# Soulfly Theme

Warm light and dark themes for [Zed](https://zed.dev), created by
[Aleksandr Ovcharenko (@pridees)](https://github.com/pridees).

Includes two variants:

- **Soulfly Dark**: near-black surfaces, soft neutral text, sand keywords,
  rose properties, blue functions, violet types, and green strings.
- **Soulfly Light**: warm ivory surfaces, dark brown text, ochre keywords,
  rose properties, blue functions, violet types, and green strings.

Both variants include matching editor, interface, diagnostic, collaboration,
and integrated terminal colors.

![Soulfly Dark in Zed with TypeScript syntax highlighting](assets/soulfly-dark.png)

The screenshot shows Soulfly Dark in the Zed IDE window with background
transparency enabled.

## Install

After the extension is published in the Zed registry:

1. Open **Extensions** in Zed and search for **Soulfly Theme**.
2. Install the extension.
3. Run **theme selector: toggle** from the command palette and select
   **Soulfly Dark** or **Soulfly Light**.

## Try the themes locally

1. Clone this repository.
2. Open Zed's command palette and run **zed: install dev extension**.
3. Select the repository directory containing `extension.toml`.
4. Open the theme selector and choose **Soulfly Dark** or **Soulfly Light**.

Alternatively, copy `themes/soulfly-dark.json` and `themes/soulfly-light.json`
to `~/.config/zed/themes/` (Linux or macOS), then select either variant in Zed.

## Follow system appearance

To switch between the two variants with your system appearance, add this to
Zed's `settings.json`:

```json
{
  "theme": {
    "mode": "system",
    "light": "Soulfly Light",
    "dark": "Soulfly Dark"
  }
}
```

## Palette

| Role | Soulfly Dark | Soulfly Light |
| --- | --- | --- |
| Editor background | `#090908` | `#faf6ee` |
| Editor foreground | `#c4beb3` | `#443b33` |
| Accent | `#ac6766` | `#8c4e54` |
| Keywords | `#ECC18E` | `#855a2b` |
| Properties | `#E58EA5` | `#924a65` |
| Functions | `#72bfff` | `#2d6487` |
| Types | `#c792ff` | `#72558d` |
| Strings | `#b5d86d` | `#486537` |
| Numbers | `#d9976e` | `#9a4e2d` |

## Publishing

See [PUBLISHING.md](PUBLISHING.md) for the Zed registry submission process.

## License

Copyright (c) 2026 Aleksandr Ovcharenko. Released under the [MIT License](LICENSE).
