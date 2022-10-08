# run `:PackerCompile` afterwards
### lua/plugins/configs/mason.lua
```lua
ensure_installed = { "lua-language-server" , "rust-analyzer"},
```


### lua/plugins/configs/lspconfig.lua
```lua
lspconfig.rust_analyzer.setup{
  settings = {
    ["rust-analyzer"] = {
      workspace = {
        symbol = {
          search = {
            kind = "all_symbols"
          }
        }
      }
    },
  }
}
```

### lua/plugins/configs/treesitter.lua
```lua
ensure_installed = {
  "lua",
  "rust",
},
```
