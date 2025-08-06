# Helix Editor Cheat Sheet

## Theme & Visual
- **Theme**: `onedark` (alternatives: `gruvbox`, `catppuccin_mocha`, `dracula`, `tokyonight`)
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
| `Ctrl+E` | File explorer (alternative) | Normal |

## Space Leader Commands - Basic Operations
| Key | Action |
|-----|--------|
| `Space q` | Quit (`:q`) |
| `Space x` | Save & quit (`:wq`) |
| `Space Q` | Force quit (`:q!`) |
| `Space W` | Write all (`:wa`) |
| `Space f` | File picker |
| `Space b` | Buffer picker |
| `Space s` | Symbol picker |
| `Space S` | Workspace symbol picker |
| `Space j` | Jump list picker |
| `Space '` | Last picker |
| `Space d` | Diagnostics picker |
| `Space D` | Workspace diagnostics picker |
| `Space r` | Rename symbol |
| `Space a` | Code action |
| `Space /` | Toggle comments |
| `Space ?` | Command palette |
| `Space k` | Hover documentation |

## Claude Code AI Integration (Space + c)
| Key | Action |
|-----|--------|
| `Space c c` | Launch Claude Code in new window |
| `Space c C` | Launch Claude Code in split pane |
| `Space c i` | Interactive Claude Code session |
| `Space c r` | Resume Claude Code session |
| `Space c h` | Claude Code help |
| `Space c s` | List Claude Code sessions |
| `Space c n` | New Claude Code session |
| `Space c f` | Analyze current file with AI |
| `Space c e` | Edit current file with AI |
| `Space c d` | Show AI diff suggestions |

## Git Operations (Space + Shift+G)
| Key | Action |
|-----|--------|
| `Space G g` | Open LazyGit in new window |
| `Space G s` | Open LazyGit in split pane |
| `Space G t` | Git status |
| `Space G d` | Git diff |
| `Space G l` | Git log |
| `Space G c` | Git commit |
| `Space G p` | Git pull |
| `Space G P` | Git push |
| `Space G b` | Git branches |
| `Space G f` | Global search (grep) |

## File Explorer (Space + e)
| Key | Action |
|-----|--------|
| `Space e e` | File explorer in split |
| `Space e E` | File explorer in new window |
| `Space e v` | File explorer vertical split |
| `Space e h` | File explorer (30% width) |
| `Space e t` | Tree view |

## Terminal/Tmux Integration (Space + t)
| Key | Action |
|-----|--------|
| `Space t t` | Terminal right (40% width) |
| `Space t T` | Terminal in new tab |
| `Space t v` | Vertical split (right) |
| `Space t h` | Horizontal split (below) |
| `Space t b` | Bottom terminal (30% height) |
| `Space t r` | Right terminal (30% width) |
| `Space t j` | Go to pane below |
| `Space t k` | Go to pane above |
| `Space t l` | Go to pane right |
| `Space t H` | Go to pane left |
| `Space t x` | Kill current pane |
| `Space t z` | Zoom/unzoom pane |
| `Space t s` | Swap with next pane |
| `Space t n` | New Helix in split |
| `Space t N` | New Helix in tab |
| `Space t c` | New window/tab |

## Run Commands (Space + Shift+R)
| Key | Action |
|-----|--------|
| `Space R n` | npm run dev |
| `Space R N` | npm dev in new tab |
| `Space R s` | npm start |
| `Space R t` | npm test |
| `Space R b` | npm build |
| `Space R i` | npm install |
| `Space R p` | Python REPL |
| `Space R P` | Run main.py |
| `Space R m` | make |
| `Space R M` | make clean && make |
| `Space R d` | docker ps |
| `Space R D` | docker-compose up |

## Window Management (Space + w)
| Key | Action |
|-----|--------|
| `Space w w` | Write/save |
| `Space w v` | Vertical split (Helix internal) |
| `Space w h` | Horizontal split (Helix internal) |
| `Space w c` | Close buffer |
| `Space w C` | Force close buffer |
| `Space w o` | Close other buffers |
| `Space w n` | New buffer |

## System Monitoring (Space + m)
| Key | Action |
|-----|--------|
| `Space m m` | htop/top |
| `Space m M` | htop in new window |
| `Space m d` | Disk usage (df -h) |
| `Space m D` | ncdu disk usage |
| `Space m n` | Network ports |
| `Space m l` | System logs |
| `Space m p` | Process list |

## Quick Access (Space + o)
| Key | Action |
|-----|--------|
| `Space o q` | Quick terminal at bottom |
| `Space o Q` | Quick terminal at right |
| `Space o z` | Open file with fzf |
| `Space o r` | Reload bashrc |
| `Space o k` | Open Helix config |
| `Space o K` | Open tmux config |
| `Space o l` | Open Helix log |
| `Space o H` | Helix help |

## Go-to Commands (g prefix)
| Key | Action |
|-----|--------|
| `g d` | Go to definition |
| `g r` | Go to reference |
| `g i` | Go to implementation |
| `g t` | Go to type definition |
| `g n` | Go to next diagnostic |
| `g p` | Go to previous diagnostic |
| `g h` | Go to line start |
| `g l` | Go to line end |

## Insert Mode
| Key | Action |
|-----|--------|
| `Ctrl+S` | Save and stay in insert mode |
| `Escape` | Return to normal mode |

## Selection Mode
| Key | Action |
|-----|--------|
| `Tab` | Indent selection |
| `Shift+Tab` | Unindent selection |
| `d` | Delete selection |
| `c` | Change selection |
| `y` | Yank (copy) |
| `/` | Toggle comments |

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

## Quick Reference Summary
- `Space f` - Find files
- `Space G g` - Git (LazyGit)
- `Space e e` - File explorer
- `Space t t` - New terminal
- `Space c c` - Claude Code AI
- `Space R n` - Run npm dev
- `Space m m` - System monitor
- `Space w v` - Split window

## Installation Requirements
1. **tmux**: `sudo apt install tmux`
2. **File managers**: `sudo apt install lf ranger nnn`
3. **LazyGit**: [Installation Guide](https://github.com/jesseduffield/lazygit)
4. **Claude Code**: [Anthropic Claude Code CLI](https://claude.ai/code)
5. **Monitoring tools**: `sudo apt install htop ncdu`
6. **fzf**: `git clone --depth 1 https://github.com/junegunn/fzf.git ~/.fzf && ~/.fzf/install`

## Tmux Basics
- `Ctrl+a d`: Detach from tmux
- `tmux a`: Reattach to tmux
- `Alt+Arrow`: Navigate panes (if configured)