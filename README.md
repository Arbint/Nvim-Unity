# Nvim Unity Configuration

A complete, modern Neovim configuration specifically optimized for Unity and C# development. This setup transforms Neovim into a powerful IDE-like experience with intelligent code completion, debugging, and seamless Unity integration.

## ✨ Features

- **🎯 C# LSP Support**: OmniSharp integration with full IntelliSense, go-to-definition, and error checking
- **🎮 Unity Development**: Optimized workflows for Unity projects with debugging support
- **🔍 Fuzzy Finding**: Telescope integration for lightning-fast file and text searching
- **💡 Smart Completion**: nvim-cmp with context-aware suggestions and snippets
- **🐛 Advanced Debugging**: DAP with NetCoreDbg for Unity and .NET debugging
- **📁 File Management**: Neo-tree file explorer with git integration
- **🎨 Modern UI**: Beautiful Tokyo Night theme with smooth animations
- **⚡ Performance**: Lazy loading for fast startup times
- **🔗 Git Integration**: Gitsigns and diffview for comprehensive version control

## 📦 Plugins Overview

### Core Framework
- **[lazy.nvim](https://github.com/folke/lazy.nvim)** - Modern plugin manager with lazy loading
- **[plenary.nvim](https://github.com/nvim-lua/plenary.nvim)** - Lua utility functions

### Language Server Protocol (LSP)
- **[nvim-lspconfig](https://github.com/neovim/nvim-lspconfig)** - LSP configuration helper
- **[mason.nvim](https://github.com/williamboman/mason.nvim)** - Package manager for LSP servers
- **[mason-lspconfig.nvim](https://github.com/williamboman/mason-lspconfig.nvim)** - Bridge between Mason and lspconfig
- **[fidget.nvim](https://github.com/j-hui/fidget.nvim)** - LSP progress notifications
- **[neodev.nvim](https://github.com/folke/neodev.nvim)** - Enhanced Lua LSP for Neovim config

### Code Completion
- **[nvim-cmp](https://github.com/hrsh7th/nvim-cmp)** - Completion engine
- **[cmp-nvim-lsp](https://github.com/hrsh7th/cmp-nvim-lsp)** - LSP completion source
- **[cmp-buffer](https://github.com/hrsh7th/cmp-buffer)** - Buffer completion source
- **[cmp-path](https://github.com/hrsh7th/cmp-path)** - File path completion
- **[cmp-cmdline](https://github.com/hrsh7th/cmp-cmdline)** - Command line completion
- **[LuaSnip](https://github.com/L3MON4D3/LuaSnip)** - Snippet engine
- **[cmp_luasnip](https://github.com/saadparwaiz1/cmp_luasnip)** - Snippet completion source
- **[friendly-snippets](https://github.com/rafamadriz/friendly-snippets)** - Pre-built snippets

### File Navigation & Search
- **[telescope.nvim](https://github.com/nvim-telescope/telescope.nvim)** - Fuzzy finder and live grep
- **[telescope-fzf-native.nvim](https://github.com/nvim-telescope/telescope-fzf-native.nvim)** - FZF integration for faster searching
- **[neo-tree.nvim](https://github.com/nvim-neo-tree/neo-tree.nvim)** - File explorer with git integration
- **[nvim-web-devicons](https://github.com/nvim-tree/nvim-web-devicons)** - File type icons

### Debugging
- **[nvim-dap](https://github.com/mfussenegger/nvim-dap)** - Debug Adapter Protocol client
- **[nvim-dap-ui](https://github.com/rcarriga/nvim-dap-ui)** - UI for nvim-dap
- **[nvim-dap-virtual-text](https://github.com/theHamsta/nvim-dap-virtual-text)** - Virtual text for debugging
- **[nvim-nio](https://github.com/nvim-neotest/nvim-nio)** - Async I/O library

### Syntax & Treesitter
- **[nvim-treesitter](https://github.com/nvim-treesitter/nvim-treesitter)** - Syntax highlighting and parsing
- **[nvim-treesitter-textobjects](https://github.com/nvim-treesitter/nvim-treesitter-textobjects)** - Text objects for treesitter

### Git Integration
- **[gitsigns.nvim](https://github.com/lewis6991/gitsigns.nvim)** - Git decorations and hunk management
- **[diffview.nvim](https://github.com/sindrets/diffview.nvim)** - Git diff viewer

### UI & Theme
- **[tokyonight.nvim](https://github.com/folke/tokyonight.nvim)** - Modern color scheme
- **[lualine.nvim](https://github.com/nvim-lualine/lualine.nvim)** - Status line
- **[alpha-nvim](https://github.com/goolord/alpha-nvim)** - Start screen
- **[indent-blankline.nvim](https://github.com/lukas-reineke/indent-blankline.nvim)** - Indentation guides
- **[noice.nvim](https://github.com/folke/noice.nvim)** - Enhanced UI for messages and command line
- **[nvim-notify](https://github.com/rcarriga/nvim-notify)** - Notification manager

### Editor Enhancements
- **[which-key.nvim](https://github.com/folke/which-key.nvim)** - Keybinding hints
- **[flash.nvim](https://github.com/folke/flash.nvim)** - Enhanced navigation and search
- **[neoscroll.nvim](https://github.com/karb94/neoscroll.nvim)** - Smooth scrolling animations
- **[conform.nvim](https://github.com/stevearc/conform.nvim)** - Code formatting
- **[mini.nvim](https://github.com/echasnovski/mini.nvim)** modules:
  - **mini.pairs** - Auto-close brackets and quotes
  - **mini.comment** - Smart commenting
  - **mini.ai** - Enhanced text objects
  - **mini.surround** - Surround text objects
  - **mini.bufremove** - Better buffer deletion
- **[vim-illuminate](https://github.com/RRethy/vim-illuminate)** - Highlight word under cursor
- **[nvim-ts-context-commentstring](https://github.com/JoosepAlviste/nvim-ts-context-commentstring)** - Context-aware commenting

## ⌨️ Key Bindings

### Leader Key
- **Leader**: `<Space>` (spacebar)

### File Navigation
| Key | Action | Description |
|-----|--------|-------------|
| `<Space>ff` | Find Files | Fuzzy find files in project |
| `<Space><Space>` | Find Files | Alternative find files |
| `<Space>/` | Live Grep | Search text in all files |
| `<Space>sg` | Live Grep | Alternative live grep |
| `<Space>fb` | Find Buffers | List open buffers |
| `<Space>,` | Switch Buffer | Quick buffer switcher |
| `<Space>fr` | Recent Files | Recently opened files |
| `<Space>fR` | Recent (CWD) | Recent files in current directory |
| `<Space>e` | Toggle Neo-tree | File explorer |
| `<Space>fe` | Toggle Neo-tree | Alternative file explorer |
| `<Space>fE` | Reveal File | Reveal current file in tree |

### LSP Features
| Key | Action | Description |
|-----|--------|-------------|
| `gd` | Go to Definition | Jump to symbol definition |
| `gr` | Go to References | Find all references |
| `gi` | Go to Implementation | Jump to implementation |
| `gt` | Go to Type Definition | Jump to type definition |
| `K` | Hover Documentation | Show symbol documentation |
| `<Space>rn` | Rename Symbol | Rename symbol across project |
| `<Space>ca` | Code Actions | Show available code actions |
| `<Space>cf` | Format Buffer | Format current buffer |
| `<Space>cd` | Line Diagnostics | Show diagnostics for current line |

### Debugging
| Key | Action | Description |
|-----|--------|-------------|
| `<Space>db` | Toggle Breakpoint | Set/remove breakpoint |
| `<Space>dB` | Conditional Breakpoint | Set conditional breakpoint |
| `<Space>dc` | Continue | Continue debugging |
| `<Space>di` | Step Into | Step into function |
| `<Space>do` | Step Out | Step out of function |
| `<Space>dO` | Step Over | Step over line |
| `<Space>dr` | Toggle REPL | Open debug REPL |
| `<Space>dt` | Terminate | Stop debugging |
| `<Space>dw` | Debug Widgets | Show debug widgets |

### Window Navigation
| Key | Action | Description |
|-----|--------|-------------|
| `<Ctrl>h` | Left Window | Move to left split |
| `<Ctrl>j` | Down Window | Move to lower split |
| `<Ctrl>k` | Up Window | Move to upper split |
| `<Ctrl>l` | Right Window | Move to right split |
| `<Ctrl>Up` | Resize Up | Increase window height |
| `<Ctrl>Down` | Resize Down | Decrease window height |
| `<Ctrl>Left` | Resize Left | Decrease window width |
| `<Ctrl>Right` | Resize Right | Increase window width |

### Buffer Management
| Key | Action | Description |
|-----|--------|-------------|
| `<Shift>h` | Previous Buffer | Switch to previous buffer |
| `<Shift>l` | Next Buffer | Switch to next buffer |
| `<Space>bd` | Delete Buffer | Close current buffer |
| `<Space>bD` | Force Delete | Force close buffer |
| `<Space>bb` | Other Buffer | Switch to other buffer |

### Text Editing
| Key | Action | Description |
|-----|--------|-------------|
| `jk` | Exit Insert | Exit insert mode |
| `<Alt>j` | Move Line Down | Move current line down |
| `<Alt>k` | Move Line Up | Move current line up |
| `<Ctrl>s` | Save File | Save current file |
| `s` | Flash Jump | Quick jump to location |
| `S` | Flash Treesitter | Treesitter-aware jump |
| `gsa` | Add Surrounding | Add surrounding characters |
| `gsd` | Delete Surrounding | Remove surrounding characters |
| `gsr` | Replace Surrounding | Replace surrounding characters |

### Git Integration
| Key | Action | Description |
|-----|--------|-------------|
| `]h` | Next Hunk | Jump to next git hunk |
| `[h` | Previous Hunk | Jump to previous hunk |
| `<Space>ghs` | Stage Hunk | Stage current hunk |
| `<Space>ghr` | Reset Hunk | Reset current hunk |
| `<Space>ghp` | Preview Hunk | Preview hunk changes |
| `<Space>ghb` | Blame Line | Show git blame |
| `<Space>gd` | Git Diff | Open diff view |

### Search & Replace
| Key | Action | Description |
|-----|--------|-------------|
| `<Space>sh` | Help Tags | Search help documentation |
| `<Space>sk` | Keymaps | Search keybindings |
| `<Space>sc` | Commands | Search available commands |
| `<Space>ss` | Document Symbols | Search symbols in current file |
| `<Space>sS` | Workspace Symbols | Search symbols in workspace |
| `<Space>sw` | Word Under Cursor | Search word under cursor |

### Diagnostics
| Key | Action | Description |
|-----|--------|-------------|
| `]d` | Next Diagnostic | Jump to next diagnostic |
| `[d` | Previous Diagnostic | Jump to previous diagnostic |
| `]e` | Next Error | Jump to next error |
| `[e` | Previous Error | Jump to previous error |
| `]w` | Next Warning | Jump to next warning |
| `[w` | Previous Warning | Jump to previous warning |

### Completion
| Key | Action | Description |
|-----|--------|-------------|
| `<Enter>` | Accept Completion | Confirm selected completion |
| `<Ctrl>n` | Next Item | Select next completion |
| `<Ctrl>p` | Previous Item | Select previous completion |
| `<Ctrl>Space>` | Trigger Completion | Manually trigger completion |
| `<Ctrl>e` | Abort | Cancel completion |

## 🚀 Installation

### Prerequisites
- **Neovim 0.9+** (0.10+ recommended for best experience)
- **Git** - For plugin management and version control
- **Node.js** - Required for some language servers
- **.NET SDK** - For C# development and OmniSharp
- **ripgrep** - For fast text searching (install via package manager)
- **make** - For building telescope-fzf-native (Windows: install via chocolatey)

### Quick Install

#### Linux/macOS
```bash
# Backup existing config
mv ~/.config/nvim ~/.config/nvim.backup

# Clone this configuration
git clone https://github.com/Arbint/Nvim-Unity.git ~/.config/nvim

# Start Neovim
nvim
```

#### Windows
```powershell
# Backup existing config
mv $env:LOCALAPPDATA\nvim $env:LOCALAPPDATA\nvim.backup

# Clone this configuration
git clone https://github.com/Arbint/Nvim-Unity.git $env:LOCALAPPDATA\nvim

# Start Neovim
nvim
```

### First-Time Setup

1. **Open Neovim** - Lazy.nvim will automatically install plugins
2. **Install Language Servers**: Run `:Mason` and install:
   - `omnisharp` (C# LSP)
   - `netcoredbg` (C# debugger)
   - `csharpier` (C# formatter)
3. **Restart Neovim** to ensure everything loads correctly
4. **Test C# Features**: Open a `.cs` file and verify LSP is working with `:LspInfo`

## 🎮 Unity Development Workflow

### Project Setup
1. **Open Unity Project**: Navigate to your Unity project root and run `nvim`
2. **LSP Attachment**: OmniSharp will automatically detect your project and provide IntelliSense
3. **File Navigation**: Use `<Space>ff` to quickly navigate between scripts
4. **Symbol Search**: Use `<Space>ss` to find classes, methods, and properties

### Debugging Unity
1. **Set Breakpoints**: Use `<Space>db` to toggle breakpoints in your scripts
2. **Attach Debugger**: Configure Unity to accept external debuggers
3. **Start Debugging**: Use `<Space>dc` to start the debugging session
4. **Debug Controls**: Use step into (`<Space>di`), step over (`<Space>dO`), and continue (`<Space>dc`)

### Code Quality
- **Auto-formatting**: Files automatically format on save with CSharpier
- **Real-time Diagnostics**: Errors and warnings appear immediately
- **Code Actions**: Use `<Space>ca` for quick fixes and refactoring
- **Symbol Renaming**: Use `<Space>rn` to rename symbols across the entire project

## 🔧 Customization

### Changing Theme
Edit `lua/plugins/ui.lua` and modify the tokyonight configuration:
```lua
opts = { style = "storm" }, -- Options: storm, moon, night, day
```

### Adding New Keybindings
Add custom keybindings in `lua/config/keymaps.lua`:
```lua
map("n", "<leader>custom", "<cmd>YourCommand<cr>", { desc = "Your Description" })
```

### Installing Additional Language Servers
1. Run `:Mason`
2. Search for your language server
3. Press `i` to install
4. Configure in `lua/plugins/lsp.lua`

## 🐛 Troubleshooting

### LSP Not Working
1. Check if you're in a C# file (`.cs` extension)
2. Run `:LspInfo` to see attached servers
3. Install OmniSharp via `:Mason`
4. Check `:LspLog` for error messages
5. Restart Neovim after installing language servers

### Telescope Not Finding Files
1. Ensure you're in a project directory
2. Install ripgrep for better performance
3. Check if git is available (Telescope uses git for file listing)

### Debugging Issues
1. Verify NetCoreDbg is installed via `:Mason`
2. Ensure your Unity project is configured for external debugging
3. Check firewall settings if debugging over network

### Performance Issues
1. Update to Neovim 0.10+ for better performance
2. Check for conflicting plugins
3. Use `:Lazy profile` to identify slow-loading plugins

## 📚 Learning Resources

- **Neovim Documentation**: `:help` or [neovim.io](https://neovim.io)
- **Vim Motions**: `:Tutor` for interactive Vim tutorial
- **LSP Features**: `:help lsp` for Language Server Protocol documentation
- **Plugin Documentation**: Use `<Space>sh` to search help for specific plugins

## 🤝 Contributing

Feel free to open issues and pull requests to improve this configuration. When contributing:

1. **Test Changes**: Ensure modifications work with Unity projects
2. **Document Updates**: Update this README for new features
3. **Follow Conventions**: Maintain consistent code style and structure

## 📄 License

This configuration is open source and available under the MIT License. Feel free to use, modify, and share!

---

**Happy Unity Development with Neovim! 🎮⚡**