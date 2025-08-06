# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is a Helix editor configuration directory containing custom settings, key bindings, and editor preferences. The configuration is designed to provide a VSCode-like experience within the Helix editor.

## Key Files Structure

- `config.toml` - Main configuration file containing theme, editor settings, and custom key bindings

## Configuration Architecture

### Theme and Visual Settings
- Uses "onedark" theme with alternatives commented for easy switching
- Configured with relative line numbers, cursor line highlighting, and rulers at columns 80/120
- Custom status line layout and cursor shapes for different modes

### Key Binding Philosophy
The configuration implements VSCode-like key bindings:
- `Ctrl+P` and `Ctrl+B` for file navigation
- `Ctrl+S` for save, `Ctrl+Q` for quit
- Extensive space-leader key bindings for quick access to commands
- Go-to commands (`gd`, `gr`, `gi`) for code navigation

### Editor Behavior
- Auto-save disabled, manual save preferred
- Mouse support and middle-click paste enabled
- Auto-formatting and auto-pairs enabled
- LSP integration with diagnostics and inlay hints

## Common Development Tasks

### Configuration Testing
```bash
# Check Helix configuration health
hx --health

# Test specific language server
hx --health <language>
```

### Configuration Validation
The main config file is TOML format. Validate syntax with:
```bash
# Check TOML syntax
helix config.toml
```

## Important Notes

- Configuration includes extensive LSP support for multiple languages
- Custom key bindings prioritize VSCode familiarity
- Theme and visual settings optimized for productivity
- Missing runtime directory may cause warnings but doesn't affect functionality

## Configuration Patterns

### Adding New Key Bindings
Key bindings follow the pattern in `[keys.normal]` and `[keys.select]` sections. Space-leader commands are defined in the `space` inline table.

### Theme Switching
Uncomment desired theme in the `[theme]` section. Available themes are documented in comments.

### LSP Configuration
Language server settings are handled through Helix's built-in language configuration system. Check `hx --health` to see available and missing language servers.