# tool_term_toggle

Toggle an i3 scratchpad/dropdown Alacritty terminal.

## Commands

- `term-toggle` - show/hide a scratchpad terminal, creating it if needed

## Dependencies

- bash
- i3-msg
- xdotool
- alacritty
- xseticon (optional, for icons)

## Install

```bash
./install.sh
```

Install to a custom prefix:

```bash
PREFIX="$HOME/.local" ./install.sh
```

## Usage

```bash
term-toggle
```

## Configuration

- Uses i3 window class `dropdown-term`.
- Icon path defaults to `$HOME/.local/share/pixmaps/dropdown-term.png`.

## Notes

These scripts were extracted from a personal Arch Linux + i3 workspace. Review dependencies and paths before using them on another machine.
