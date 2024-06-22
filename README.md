<!-- panvimdoc-ignore-start -->

<h3 align="center">
    <img src="https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/logos/exports/1544x1544_circle.png" width="100" alt="Logo"/><br/>
    <img src="https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/misc/transparent.png" height="30" width="0px"/>
    Catppuccinight
    <img src="https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/misc/transparent.png" height="30" width="0px"/>
</h3>

![round2](https://github.com/m4xshen/catppuccinight.nvim/assets/74842863/62e00c06-08df-403d-8352-e1976f8a1a94)

Don't install this plugin! Use following config instead:

```lua
{
  "catppuccin/nvim",
  name = "catppuccin",
  priority = 1000,
  opts = {
     flavour = "mocha",
     custom_highlights = function(colors)
        return {
           WinSeparator = { fg = colors.surface0 },
        }
     end,
     color_overrides = {
        mocha = {
           base = "#11111b",
           mantle = "#11111b",
        },
     },
     integrations = {
        notify = true,
     },
  },
  init = function()
     vim.cmd.colorscheme("catppuccin")
  end,
}
```
