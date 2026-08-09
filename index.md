# 各种配置

## vscode settings.json

```jsonc
// ---- clangd 基于token 高亮自定义 ----
"editor.semanticHighlighting.enabled": true,
"editor.semanticTokenColorCustomizations": {
    "enabled": true,
    "rules": {
        "type": "#3decc6",
        "struct": "#3decc6",
        "class": "#e0c988",
        "class.defaultLibrary": "#3decc6",
        "namespace": "#DCDCAA",
        "function": "#f8825f",
        "method": "#f8825f",
        "variable": "#e0edff",
        "parameter": "#e3cdf3",
        "variable.readonly": "#ec1d16",
        "variable.defaultLibrary": "#f8825f",
        "property": "#74d8f0",
        "macro": "#BD63C5",
        "enumMember": "#ec1d16"
    }
},

// 基于TextMate的纯文本 高亮自定义
"editor.tokenColorCustomizations": {
    "textMateRules": [
        { "scope": "keyword.other.using.directive.cpp", "settings": { "foreground": "#ae7feb"} },
        { "scope": "keyword.control.directive.define.cpp", "settings": { "foreground": "#8fbbfc"} },
        { "scope": "keyword.control.directive.include.cpp", "settings": { "foreground": "#8fbbfc"} },
        { "scope": "string.quoted.other.lt-gt.include.cpp", "settings": { "foreground": "#8ed7d0"} },
        { "scope": "storage.type.built-in.primitive.cpp", "settings": { "foreground": "#bd63c5"} },
        { "scope": "storage.modifier.specifier.const.cpp", "settings": { "foreground": "#bd63c5"} }
    ]
}
```

## vimrc

```vim
" --- 复制、剪切、粘贴、撤销映射 ---

" Ctrl + C: 选中状态下复制到系统剪贴板
vnoremap <C-c> "+y

" Ctrl + X: 选中状态下剪切到系统剪贴板
vnoremap <C-x> "+d

" Ctrl + V: 普通模式/插入模式/命令行模式下粘贴
nnoremap <C-v> "+p
inoremap <C-v> <C-r>+
cnoremap <C-v> <C-r>+

" Ctrl + Z: 撤销
nnoremap <C-z> u
inoremap <C-z> <C-o>u

" Ctrl + Y: 重做 (反撤销)
nnoremap <C-y> <C-r>
inoremap <C-y> <C-o><C-r>
" Ctrl + L: 清除高亮
nnoremap <silent> <C-l> :nohlsearch<CR><C-l>

set number
set clipboard=unnamedplus
set shortmess-=S " 移除 S 选项，允许在右下角显示搜索匹配数 [x/Y]
set hlsearch     " 高亮所有匹配项
set incsearch    " 边输入边实时跳转匹配
set ignorecase   " 搜索时忽略大小写
set smartcase    " 如果输入包含大写字母，自动切换为大小写敏感
```

