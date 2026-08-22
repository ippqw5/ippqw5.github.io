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


" 语法高亮度显示
syntax on

"搜索匹配高亮
set hlsearch

set cuc
set cul
" 设置行号
set nu

"防止中文注释乱码
set fileencoding=utf-8
set fenc=utf-8
set fencs=utf-8,usc-bom,euc-jp,gb18030,gbk,gb2312,cp936,big－5                    
set enc=utf-8
let &termencoding=&encoding

"设置字体
set guifont=Monospace\ 13

" 设置tab4个空格
set tabstop=4
set expandtab

"程序自动缩进时候空格数
set shiftwidth=4

"退格键一次删除4个空格
set softtabstop=4
autocmd FileType make set noexpandtab

" 在编辑过程中，在右下角显示光标位置的状态行
set ruler

" 搜索忽略大小写 
set ignorecase 

" vim使用自动对起，也就是把当前行的对起格式应用到下一行
set autoindent

" 依据上面的对起格式，智能的选择对起方式，对于类似C语言编写上很有用
set smartindent

```

