# Pirokai Beach Sunset.nvim

A dark Neovim colorscheme based on **Monokai Pirokai – Beach Sunset**.

The theme uses a near-black background with warm reds, oranges and yellows, balanced by green, cyan and purple accents.

## Requirements

- Neovim with true-color support

## Installation

### lazy.nvim

```lua
{
  "roxxel/pirokai-beach-sunset.nvim",
  priority = 1000,
  config = function()
    vim.cmd.colorscheme("pirokai-beach-sunset")
  end,
}
```

### LazyVim

```lua
return {
  {
    "roxxel/pirokai-beach-sunset.nvim",
    lazy = false,
    priority = 1000,
  },
  {
    "LazyVim/LazyVim",
    opts = {
      colorscheme = "pirokai-beach-sunset",
    },
  },
}
```

## Usage

```vim
:colorscheme pirokai-beach-sunset
```

Or from Lua:

```lua
vim.cmd.colorscheme("pirokai-beach-sunset")
```

## Palette

| Role | Color |
| --- | --- |
| Background | `#131313` |
| Foreground | `#f7f1ff` |
| Red | `#fc618d` |
| Orange | `#fd9353` |
| Yellow | `#fce566` |
| Green | `#7bd88f` |
| Cyan | `#5ad4e6` |
| Purple | `#948ae3` |

## Highlight support

Includes highlights for core Neovim UI and syntax, Treesitter, LSP semantic tokens and diagnostics, plus integrations for commonly used plugins including GitSigns, Snacks, Blink.cmp, Trouble, indent-blankline, WhichKey, Lazy.nvim, Mason and Bufferline.

## Development

The colorscheme entry point is:

```text
colors/pirokai-beach-sunset.lua
```

The implementation and palette live in:

```text
lua/pirokai_beach_sunset/
```

Reload while editing with:

```vim
:colorscheme pirokai-beach-sunset
```

Use `:Inspect` to inspect highlight groups under the cursor.
