# dawn.nvim

## Installation

### lazy.nvim

```lua
local lazy = require("lazy")

lazy.setup({
    {
        "AlphaKeks/dawn.nvim",
        config = function()
            require("dawn").setup({
                transparent = true, -- adjust this as you wish
            })

            vim.cmd.colorscheme("dawn")
        end,
    }
})
```

### packer.nvim

```lua
local packer = require("packer")

packer.setup(function(use)
    use("AlphaKeks/dawn.nvim")
end)

local dawn_installed, dawn = pcall(require, "dawn")

if dawn_installed then
    require("dawn").setup({
        transparent = true, -- adjust this as you wish
    })

    vim.cmd.colorscheme("dawn")
end
```

## Color palette

The color palette is taken from [catppuccin](https://github.com/catppuccin/nvim).
There are 2 additional colors and you can get access to the palette like this:

```lua
local dawn_palette = require("dawn").palette
```
