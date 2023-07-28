# Kitty设置字体(中文与英文字体互不干扰）
具体可查看[kitty官网](https://sw.kovidgoyal.net/kitty)

## 创建一个kitty.conf在~/.config/kitty中，写入
`
font_size 14.0 #设置字体大小
font_family Cascadia Code #设置英文字体
background_opacity 0.70 #设置窗口透明度

symbol_map U+4E00-U+9FFF,U+3400-U+4DBF Microsoft YaHei UI #指定unicode以使用中文字体显示

# keybinds

kitty_mod ctrl+shift #设置按键

map kitty_mod+c copy_to_clipboard #复制按键
map kitty_mod+v paste_from_clipboard #粘贴按键
`