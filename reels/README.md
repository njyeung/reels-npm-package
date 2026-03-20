# reels

TUI for Instagram Reels. Doomscrollbrainrotmaxxing in the terminal.

## Install

```bash
npm install -g @reels/tui
```

## Prerequisites

### Terminal
You need a terminal that supports the **Kitty graphics protocol**:
- [Kitty](https://sw.kovidgoyal.net/kitty/) (recommended)
- [WezTerm](https://wezfurlong.org/wezterm/)
- [Konsole](https://konsole.kde.org/)

### Browser
Chrome, Chromium, or Brave must be installed. The app uses headless browser automation to interact with Instagram.

### FFmpeg
FFmpeg 8+ must be installed on your system.

## Usage

```bash
reels
```

### Flags
- `--headed` - Run browser in headed mode (visible browser window)
- `--login` - Open browser window to log in to Instagram

### Controls
- `j` - Next reel (scroll comments when open)
- `k` - Previous reel (scroll comments when open)
- `Space` - Pause/resume
- `l` - Like/unlike
- `e` - Toggle Navbar
- `c` - Toggle Comments
- `m` - Mute
- `]` - Volume up
- `[` - Volume down
- `s` - Share reel via DM
- `y` - Copy reel link to clipboard
- `=` - Enlarge Video
- `-` - Shrink Video
- `?` - Help
- `q` - Quit

All keybinds are configurable in `reels.conf`. Each action supports multiple binds.

## Supported Platforms

| Platform | Package |
|----------|---------|
| Linux x64 | `@reels/linux-x64` |
| macOS ARM64 | `@reels/darwin-arm64` |

## File Paths

- Settings: `~/.config/reels/reels.conf`
- Cache: `~/.cache/reels/`
- Chrome Data: `~/.local/shared/reels/`

## Links

- [GitHub](https://github.com/njyeung/reels)
- [Homebrew](https://github.com/njyeung/homebrew-tap)
- [AUR](https://aur.archlinux.org/packages/reels-bin)
