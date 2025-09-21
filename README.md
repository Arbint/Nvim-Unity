# Nvim Unity Configuration

A complete Neovim configuration optimized for Unity and C# development.

## Features

- **C# LSP Support**: OmniSharp integration for full IntelliSense
- **Unity Development**: Optimized for Unity projects with debugging support
- **File Navigation**: Telescope for fuzzy finding and project search
- **Code Completion**: nvim-cmp with snippets and intelligent suggestions
- **Debugging**: DAP with NetCoreDbg for Unity and .NET debugging
- **Git Integration**: Gitsigns and diffview for version control
- **Modern UI**: Beautiful interface with Tokyo Night theme

## Key Bindings

### File Navigation
- `<Space>ff` - Find files
- `<Space>/` - Live grep (search in files)
- `<Space>e` - Toggle file explorer

### LSP Features
- `gd` - Go to definition
- `gr` - Find references
- `K` - Show hover documentation
- `<Space>cd` - Show diagnostics

### Debugging
- `<Space>db` - Toggle breakpoint
- `<Space>dc` - Start debugging
- `<Space>dr` - Toggle REPL

### Window Navigation
- `<Ctrl>h/j/k/l` - Navigate between panes

## Installation

1. Clone this repository to your Neovim config directory:
   ```bash
   git clone https://github.com/YOUR_USERNAME/Nvim-Unity.git ~/.config/nvim
   ```

2. Open Neovim and let Lazy.nvim install plugins:
   ```
   nvim
   ```

3. Install language servers via Mason:
   ```
   :Mason
   ```

## Requirements

- Neovim 0.9+
- Git
- Node.js (for some language servers)
- .NET SDK (for C# development)
- ripgrep (for telescope grep)

## Unity Development

This configuration is specifically optimized for Unity development with:
- C# syntax highlighting and IntelliSense
- Unity project structure recognition
- Debugging support for Unity processes
- Auto-formatting with CSharpier
- Git integration for Unity projects

Enjoy coding with Neovim! 🚀