# tool_term_toggle

Toggle an i3 scratchpad/dropdown Alacritty terminal.

## Commands

- `term-toggle` - show/hide a scratchpad terminal, creating it if needed

## Dependencies

Required shell:
- Bash

Required commands:
- `xdotool`
- `i3-msg`
- `alacritty`

Optional commands:
- `xseticon` - sets the dropdown terminal window icon

The executable scripts call `need` for required commands before using them.

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
- Includes original project icon `share/pixmaps/dropdown-term.png`; `install.sh` installs it to `${XDG_DATA_HOME:-$HOME/.local/share}/pixmaps/dropdown-term.png`.

## Notes

These scripts were extracted from a personal Arch Linux + i3 workspace. Review dependencies and paths before using them on another machine.
