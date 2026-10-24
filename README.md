# Sunset theme for ARGVUS

Official ARGVUS Dark theme, `sunset`, with its Sticky and Float variants.

[![CI](https://github.com/argvus/argvus-theme-sunset/actions/workflows/ci.yml/badge.svg)](https://github.com/argvus/argvus-theme-sunset/actions/workflows/ci.yml)
[![Release](https://github.com/argvus/argvus-theme-sunset/actions/workflows/release.yml/badge.svg)](https://github.com/argvus/argvus-theme-sunset/actions/workflows/release.yml)
[![License](https://img.shields.io/badge/License-GPL--3.0-blue.svg)](LICENSE)

## Theme identity

| Field | Value |
| --- | --- |
| Theme ID | `sunset` (Float variant: `sunset-float`) |
| Display name | Sunset |
| Mode | `dark` |
| Default highlight | `#E2BE8A` |
| GTK color scheme | `prefer-dark` |
| Calendar stylesheet | `sunset` |
| Package | `argvus-theme-sunset` |
| Wallpaper | `/usr/share/backgrounds/argvus/abstract/dark/sunset-abstract-dark.jxl` |

The values above are the ones declared in
`src/usr/share/argvus/appearance/themes.d/sunset/theme.toml`, the manifest that the
desktop reads. The manifest is the source of truth; this page describes it.

## Installing

The package depends on `argvus` and `argvus-appearance`, so pacman installs them with it.

```sh
sudo pacman -S argvus-theme-sunset
```

Select the theme in the Control Center (Appearance > Themes), or run
`argvus theme-switch sunset`.

## Files

The package installs the theme's per-component files under `/usr/share/argvus` (and the
calendar stylesheet under `/etc/argvus/taskbar/calendar/themes`). Each component that
the theme styles has its own directory, listed by `find src -type f` in this repository.

## Development

Validate with `make validate` before building. The design rules are in
[DEVELOPMENT.md](DEVELOPMENT.md); the ARGVUS documentation for themes is in
`argvus/docs/en/user-guide/appearance.md` of the `argvus` repository.

## Contributing and policies

- [CONTRIBUTING.md](https://github.com/argvus/.github/blob/main/CONTRIBUTING.md) — contribution workflow
- [SECURITY.md](https://github.com/argvus/.github/blob/main/SECURITY.md) — private vulnerability reports
- [Code of Conduct](https://github.com/argvus/.github/blob/main/policies/CODE_OF_CONDUCT.md) — community standards
- [AI usage policy](https://github.com/argvus/.github/blob/main/policies/IA_USAGE.md) — rules for AI-assisted contributions

## License

GPL-3.0-only. See [LICENSE](LICENSE).
