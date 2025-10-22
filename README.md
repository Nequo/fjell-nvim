# Fjell

Fjell is a minimal colorscheme based on [Mies](https://github.com/jaredgorski/Mies.vim) and [Mountain](https://github.com/mountain-theme/Mountain/blob/master/docs/fuji.org).

The light variant uses colors from [Modus Operandi Tinted](https://protesilaos.com/emacs/modus-themes-colors)

## Design

The theme simply uses `vim.api.nvim_set_hl` to set highlight colors and does not aim to provide any advanced customisability.
Color is only used for non-syntax elements such as LSP Diagnostics, search and menus.

## Configuration

### Alternate diffs

To use alternate colors for diffs, use the setup function:

```lua
require('fjell').setup({
  alternate_diffs = true
})
```

Alternatively:

```lua
vim.g.fjell_alternate_diffs = true
```

### Installation with lazy.nvim

Add to your `lazy.lua`:

```lua
{
  'Nequo/fjell-nvim',
  config = function()
    require('fjell').setup({
      alternate_diffs = true  -- optional
    })
    vim.cmd.colorscheme('fjell')
  end
}
```


## Screenshot
<img width="1512" height="945" alt="image" src="https://github.com/user-attachments/assets/2410145d-8207-45f0-bb7e-56509d24fa15" />
