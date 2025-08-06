# Helix Editor Cheat Sheet

## Theme & Visual
- **Theme**: `onedark` (alternatives: `gruvbox`, `catppuccin_mocha`, `dracula`)
- **Line numbers**: Relative
- **Cursor line**: Highlighted
- **Rulers**: At columns 80 and 120
- **Status bar**: Mode, file info (left) | diagnostics, position (right)

## Quick Actions
| Key | Action | Mode |
|-----|--------|------|
| `Ctrl+S` | Save file | Normal/Insert |
| `Ctrl+Q` | Quit | Normal |
| `Ctrl+P` | File picker | Normal |
| `Ctrl+B` | File browser | Normal |

## Space Leader Commands
| Key | Action |
|-----|--------|
| `Space w` | Save (`:w`) |
| `Space q` | Quit (`:q`) |
| `Space x` | Save & quit (`:wq`) |
| `Space f` | File picker |
| `Space b` | Buffer picker |
| `Space s` | Symbol picker |
| `Space S` | Workspace symbol picker |
| `Space r` | Rename symbol |
| `Space a` | Code action |
| `Space h` | Hover info |
| `Space /` | Toggle comments |

## File Management
| Key | Action |
|-----|--------|
| `Space e` | Open file manager (lf) in tmux pane |

## Git Operations
| Key | Action |
|-----|--------|
| `Space g g` | Open lazygit in tmux pane |
| `Space g s` | Global search |

## Tmux Integration
| Key | Action |
|-----|--------|
| `Space t v` | Open file in vertical tmux pane |
| `Space t h` | Open file in horizontal tmux pane |
| `Space t w` | Open file in new tmux window |
| `Space t t` | Open terminal in tmux pane |

## Go-to Commands
| Key | Action |
|-----|--------|
| `g d` | Go to definition |
| `g r` | Go to reference |
| `g i` | Go to implementation |

## Selection Mode
| Key | Action |
|-----|--------|
| `Tab` | Indent selection |
| `Shift+Tab` | Unindent selection |

## Editor Features
- **Auto-save**: Disabled (manual save preferred)
- **Auto-pairs**: Enabled (brackets, quotes)
- **Auto-format**: Enabled
- **Mouse support**: Enabled
- **Middle-click paste**: Enabled
- **LSP**: Diagnostics and inlay hints enabled
- **Indent guides**: Enabled with `┊` character
- **Soft wrap**: Enabled

## Cursor Shapes
- **Normal mode**: Block cursor
- **Insert mode**: Bar cursor
- **Select mode**: Underline cursor

## Configuration Tips
- Hidden files shown in file picker
- Completion triggers after 2 characters
- Scroll 3 lines at a time
- 400ms idle timeout