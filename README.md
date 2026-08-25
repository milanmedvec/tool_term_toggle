# tool_term_toggle

Toggle an i3 scratchpad/dropdown Alacritty terminal.

## Commands

- `term-toggle` - show/hide a scratchpad terminal, creating it if needed

## Dependencies

Required commands:
- `bash`
- `i3-msg`
- `xdotool`
- `alacritty`

Optional commands:
- `xseticon` - sets the dropdown terminal window icon

Check required commands in your shell:

```bash
need() {
    command -v "$1" >/dev/null || echo "missing: $1"
}

for cmd in bash i3-msg xdotool alacritty; do
    need "$cmd"
done
```

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
