# nvim-config

My daily-driver Neovim setup, built on [AstroNvim v6](https://astronvim.com/) and configured in Lua.

![Screenshot of the editor](docs/screenshot.png)
<!-- TODO: add docs/screenshot.png -->

## What's in it
- **Language packs** from AstroCommunity for Lua, Markdown, Python, Swift and Rust: LSP, Treesitter, formatting, and debugging where the pack provides it.
- **Completion and navigation:** blink.cmp with friendly-snippets, fzf-lua/Telescope pickers, neo-tree and oil.nvim for files.
- **Apple development:** xcodebuild.nvim for building and running Xcode projects from Neovim.
- **Notes:** obsidian.nvim and render-markdown for working in my Obsidian vault.
- **Themes:** 16 colorschemes in `lua/colorschemes/`, switchable live with themery.nvim.
- Git blame, toggleterm, which-key, and custom keymaps in `lua/keymaps.lua`.

## Layout
```
init.lua            -- bootstraps lazy.nvim
lua/lazy_setup.lua  -- AstroNvim (pinned to ^6) + plugin imports
lua/community.lua   -- AstroCommunity language packs
lua/plugins/        -- one file per plugin override
lua/colorschemes/   -- theme specs
lazy-lock.json      -- pinned plugin versions
```

## Install
Requires git and a Neovim version supported by [AstroNvim](https://docs.astronvim.com/#-requirements). Back up any existing config first.
```bash
git clone https://github.com/amcnutt1996/nvim-config ~/.config/nvim
nvim   # lazy.nvim installs plugins on first launch
```

## License
[MIT](LICENSE)
