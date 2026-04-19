<p align="center">
  <img src="https://raw.githubusercontent.com/njyeung/reels/main/assets/banner.svg" alt="REELS TUI" width="100%">
</p>
<p align="center">
  <img src="https://raw.githubusercontent.com/njyeung/reels/main/assets/demo_popos.gif" width="35%" />
  <img src="https://raw.githubusercontent.com/njyeung/reels/main/assets/demo_macos.gif" width="35%">
  <img src="https://raw.githubusercontent.com/njyeung/reels/main/assets/demo_arch.gif" width="26%" />
</p>
<p align="center">
  <img src="https://raw.githubusercontent.com/njyeung/reels/main/assets/subtitle.svg" alt="Doomscrollbrainrotmaxxing in the terminal" width="500">
</p>

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

### Chrome (LINUX ARM64 ONLY)
Chrome is automatically downloaded on first run if no system Chrome/Chromium is found; No action is needed for most platforms. The exception is Linux ARM64, where Chrome For Testing isn't available yet ([coming Q2 2026!](https://blog.chromium.org/2026/03/bringing-chrome-to-arm64-linux-devices.html)). If you are on Linux ARM64, you'll need to install Chromium manually before running Reels.


## Usage

```bash
reels
```

### Flags
- `--headed` - Run browser in headed mode (visible browser window)
- `--login` - Open browser window to log in to Instagram

### Controls

| reels.conf bind | Default | Action |
|-----------------|---------|--------|
| `key_next` | `j` | Next reel (scrolls panels when open) |
| `key_previous` | `k` | Previous reel (scrolls panels when open) |
| `key_seek_backward` | `h` | Seek backward by 5 seconds |
| `key_seek_forward` | `l` | Seek forward by 5 seconds |
| `key_like` | `space` | Like/unlike |
| `key_repost` | `r` | Repost/unrepost current reel |
| `key_share_select` | `space` | Select friend in share panel. Overrides any other bind while share panel is open |
| `key_pause` | `p` | Pause/resume current reel |
| `key_save` | `b` | Save/Unsave (bookmark) current reel |
| `key_navbar` | `e` | Toggle navbar, a condensed version of the help menu |
| `key_comments_open` | `c` | Open comments |
| `key_comments_close` | `C` | Close comments |
| `key_share_open` | `s` | Open share panel. Allows you to share reels with instagram's suggested top friends. |
| `key_share_close` | `S` | Close Share panel & sends to friends' DMs (if any are selected) |
| `key_copy_link` | `y` | Copy reel link to clipboard |
| `key_mute` | `m` | Mute current reel |
| `key_vol_up` | `]` | Volume up |
| `key_vol_down` | `[` | Volume down |
| `key_reel_size_inc` | `=` | Enlarge video |
| `key_reel_size_dec` | `-` | Shrink video |
| `key_help_open` | `?` | Help panel shows the current keybinds |
| `key_help_close`| `?` | Close help panel |
| `key_quit` | `q` | Quit |
| `key_quit` | `ctrl+c` | Quit |

All keybinds are configurable in `reels.conf`. Each action supports multiple binds. Open/close pairs (like `key_comments_open` and `key_comments_close`) can be bound to the same key to toggle.

## Supported Platforms

| Platform | Package |
|----------|---------|
| Linux x64 | `@reels/linux-x64` |
| Linux ARM64 | `@reels/linux-arm64` |
| macOS ARM64 | `@reels/darwin-arm64` |

## File Paths

- Settings: `~/.config/reels/reels.conf`
- Cache: `~/.cache/reels/`
- Chrome Data: `~/.local/shared/reels/`

## Links

- [GitHub](https://github.com/njyeung/reels)
- [Homebrew](https://github.com/njyeung/homebrew-tap)
- [AUR](https://aur.archlinux.org/packages/reels-bin)
