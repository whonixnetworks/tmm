# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.0] - 2026-04-17

### Added
- Initial release of tm — tmux session manager
- Interactive session management with keyboard-driven menu
- Session creation, attachment, and management functionality
- Session renaming capability
- Bulk session termination (kill all sessions)
- Automatic shell detection for alias installation (.bashrc, .zshrc, .config/fish/config.fish)
- Support for both inside and outside tmux session contexts
- Color-coded terminal output using gum styling
- Installation script for easy setup to `/usr/local/bin/tm`
- Version information display via `tm --version`

### Features
- **Interactive Menu**: Arrow key navigation with visual feedback
- **Smart Session Handling**: Automatically detects if session exists and attaches or creates accordingly
- **Context-Aware**: Uses `switch-client` when inside tmux, `attach-session` when outside
- **Confirmation Prompts**: Safety confirmations for destructive actions (kill sessions)
- **Session Information Display**: Shows session details including creation time and window count
- **Keyboard Shortcuts**: Quick access to common actions (o=open, c=close, r=rename, n=new, q=quit)

### Dependencies
- tmux (terminal multiplexer)
- gum (interactive CLI tool by Charmbracelet)

### Installation
- Single file installation script
- Automatic shell alias setup
- Cross-platform shell support (bash, zsh, fish)

### Documentation
- Comprehensive README with usage examples
- Inline code documentation with clear section headers
- Interactive menu key bindings reference