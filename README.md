# Neon Wave

A neon-wave Sphinx theme with neon grid styling and dark/light/system modes.

## Install

```bash
pip install -e /path/to/neon-wave
```

Or in `requirements.txt`:

```
-e ../themes/neon-wave
```

## Usage

```python
html_theme = "neon-wave"

html_theme_options = {
    "light_logo": "logo-light.svg",
    "dark_logo": "logo-dark.svg",
    "sidebar_hide_name": False,
    "navigation_with_keys": True,
    "default_theme": "system",
}
```

## Theme options

- `light_logo`: logo for light mode
- `dark_logo`: logo for dark mode
- `sidebar_hide_name`: hide project name in the sidebar
- `navigation_with_keys`: enable keyboard navigation
- `default_theme`: `"dark"`, `"light"`, or `"system"`

Logo files are expected under `_static/` (for example, `_static/logo-light.svg`).

## Environment variables

These are read in the book build and passed into the theme.

- `NEONBOOK_THEME`: `neon-synth` or `neon-wave` (default: `neon-synth`)
- `NEONBOOK_VHS`: toggle VHS effects (default: `on`)
- `NEONBOOK_PERF_LOG`: enable performance console logging (default: `off`)
- `NEONBOOK_PERF_SOUND`: play a siren on heavy load (default: `off`)
- `NEONBOOK_PERF_NOTIFY`: desktop notification on heavy load (default: `off`)

For boolean flags, any value other than `0`, `off`, `false`, or `no` is treated as on.

## License

Apache License 2.0. See `LICENSE`.
