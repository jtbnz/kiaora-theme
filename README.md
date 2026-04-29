# Kiaora Theme for OpenCode

A custom [OpenCode](https://opencode.ai) theme inspired by the landscapes of Aotearoa New Zealand -- glacial lakes, pounamu jade, dusky fjords, native bush, and overcast southern skies.

Light mode uses a soft grey background (`#D8DEE9`) with subtle mint and dusky blue accents. Dark mode shifts to deep slate tones while keeping the same natural palette.

---

## Colour Palette

### Core Backgrounds

| Swatch | Name | Hex | Inspiration |
|--------|------|-----|-------------|
| ![#D8DEE9](https://via.placeholder.com/24/D8DEE9/D8DEE9?text=+) | Cloud | `#D8DEE9` | Overcast sky, light background |
| ![#CDD5E0](https://via.placeholder.com/24/CDD5E0/CDD5E0?text=+) | Mist | `#CDD5E0` | Panel background |
| ![#C4CDD9](https://via.placeholder.com/24/C4CDD9/C4CDD9?text=+) | Fog | `#C4CDD9` | Element background |
| ![#E5E9F0](https://via.placeholder.com/24/E5E9F0/E5E9F0?text=+) | Overcast | `#E5E9F0` | Diff context |
| ![#ECEFF4](https://via.placeholder.com/24/ECEFF4/ECEFF4?text=+) | Snow | `#ECEFF4` | Brightest surface |

### Dark Backgrounds

| Swatch | Name | Hex | Inspiration |
|--------|------|-----|-------------|
| ![#2E3440](https://via.placeholder.com/24/2E3440/2E3440?text=+) | Slate | `#2E3440` | Deep night sky |
| ![#3B4252](https://via.placeholder.com/24/3B4252/3B4252?text=+) | Slate Light | `#3B4252` | Dark mode panel |
| ![#434C5E](https://via.placeholder.com/24/434C5E/434C5E?text=+) | Slate Mid | `#434C5E` | Dark mode element |
| ![#4C566A](https://via.placeholder.com/24/4C566A/4C566A?text=+) | Slate Soft | `#4C566A` | Muted text (dark) |

### Accent Colours

| Swatch | Name | Hex | Inspiration |
|--------|------|-----|-------------|
| ![#8FBCBB](https://via.placeholder.com/24/8FBCBB/8FBCBB?text=+) | Pounamu | `#8FBCBB` | Jade/greenstone, mint accent |
| ![#7BAFAE](https://via.placeholder.com/24/7BAFAE/7BAFAE?text=+) | Glacial | `#7BAFAE` | Glacial lake teal (primary) |
| ![#88C0D0](https://via.placeholder.com/24/88C0D0/88C0D0?text=+) | Clear Sky | `#88C0D0` | Clear southern sky |
| ![#81A1C1](https://via.placeholder.com/24/81A1C1/81A1C1?text=+) | Dusky Blue | `#81A1C1` | Twilight over mountains |
| ![#6E8FAD](https://via.placeholder.com/24/6E8FAD/6E8FAD?text=+) | Deep Fjord | `#6E8FAD` | Milford Sound depths |
| ![#5E81AC](https://via.placeholder.com/24/5E81AC/5E81AC?text=+) | Fjord | `#5E81AC` | Deep water blue |

### Semantic Colours

| Swatch | Name | Hex | Inspiration |
|--------|------|-----|-------------|
| ![#A3BE8C](https://via.placeholder.com/24/A3BE8C/A3BE8C?text=+) | Bush | `#A3BE8C` | Native bush, silver fern |
| ![#BF616A](https://via.placeholder.com/24/BF616A/BF616A?text=+) | Pohutukawa | `#BF616A` | NZ Christmas tree red |
| ![#EBCB8B](https://via.placeholder.com/24/EBCB8B/EBCB8B?text=+) | Tussock | `#EBCB8B` | Golden tussock grass |
| ![#D08770](https://via.placeholder.com/24/D08770/D08770?text=+) | Kowhai | `#D08770` | Kowhai blossom, warning |
| ![#B48EAD](https://via.placeholder.com/24/B48EAD/B48EAD?text=+) | Manuka | `#B48EAD` | Manuka flower, numbers |

---

## Installation

### Option 1 -- User-wide (recommended)

Copy the theme file into your OpenCode config directory so it is available in every project.

```bash
# Create the themes directory if it doesn't exist
mkdir -p ~/.config/opencode/themes

# Copy the theme file
cp kiaora.json ~/.config/opencode/themes/kiaora.json
```

### Option 2 -- Per-project

Place the theme file inside your project so it only applies there.

```bash
# From your project root
mkdir -p .opencode/themes

# Copy the theme file
cp /path/to/kiaora.json .opencode/themes/kiaora.json
```

### Activate the theme

**Method A -- Command palette**

1. Open OpenCode
2. Type `/theme`
3. Select `kiaora` from the list

**Method B -- Config file**

Create or edit `tui.json` in your OpenCode config directory (`~/.config/opencode/tui.json` or `<project-root>/.opencode/tui.json`):

```json
{
  "$schema": "https://opencode.ai/tui.json",
  "theme": "kiaora"
}
```

---

## Requirements

Your terminal must support **truecolor** (24-bit colour) for the palette to render accurately.

```bash
# Check support
echo $COLORTERM
# Should output: truecolor or 24bit

# If not set, add to your shell profile
export COLORTERM=truecolor
```

Compatible terminals: iTerm2, Alacritty, Kitty, Windows Terminal, WezTerm, GNOME Terminal (recent).

---

## Theme Mapping Quick Reference

| Role | Light | Dark |
|------|-------|------|
| **Primary** | Fjord `#5E81AC` | Glacial `#7BAFAE` |
| **Secondary** | Dusky Blue `#81A1C1` | Dusky Blue `#81A1C1` |
| **Accent** | Pounamu `#8FBCBB` | Pounamu `#8FBCBB` |
| **Background** | Cloud `#D8DEE9` | Slate `#2E3440` |
| **Text** | Slate `#2E3440` | Cloud `#D8DEE9` |
| **Success** | Bush `#A3BE8C` | Bush `#A3BE8C` |
| **Error** | Pohutukawa `#BF616A` | Pohutukawa `#BF616A` |
| **Warning** | Kowhai `#D08770` | Kowhai `#D08770` |
| **Info** | Fjord `#5E81AC` | Clear Sky `#88C0D0` |

---

## License

MIT
