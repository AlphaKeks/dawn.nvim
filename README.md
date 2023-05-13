# dawn.nvim

## Installation

### lazy.nvim

```lua
local lazy = require("lazy")

lazy.setup({
    {
        "AlphaKeks/dawn.nvim",
        config = function()
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

vim.cmd.colorscheme("dawn")
```
