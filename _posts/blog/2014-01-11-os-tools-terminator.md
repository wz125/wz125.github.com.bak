---
layout: post
title: 'terminator'
category: blog
tags: tools]
---


##install
sudo apt-get install terminator
mkdir -p ~/.config/terminator/  
curl https://raw.github.com/ghuntley/terminator-solarized/master/config > ~/.config/terminator/config  

## key
Ctrl-Shift-c 拷贝
Ctrl-Shift-v 粘贴
Ctrl-Shift-t 开新Tab窗口
Ctrl-Shift-o 上下拆分屏幕
Ctrl-Shift-e 左右拆分屏幕
Ctrl-Shift-w 关闭当前窗口
Ctrl-Shift-q 关闭整个终端

##env

[global_config]
    title_transmit_bg_color = "#d30102"
    focus = system
    suppress_multiple_term_dialog = True
[keybindings]
[profiles]
    [[default]]
        palette = "#073642:#dc322f:#859900:#b58900:#268bd2:#d33682:#2aa198:#eee8d5:#002b36:#cb4b16:#586e75:#657b83:#839496:#6c71c4:#93a1a1:#fdf6e3"
        copy_on_selection = True
        background_image = None
        background_darkness = 0.95
        background_type = transparent
        use_system_font = False
        cursor_color = "#eee8d5"
        foreground_color = "#839496"
        show_titlebar = False
        font = Monospace 11
        background_color = "#002b36"
    [[solarized-dark]]
        palette = "#073642:#dc322f:#859900:#b58900:#268bd2:#d33682:#2aa198:#eee8d5:#002b36:#cb4b16:#586e75:#657b83:#839496:#6c71c4:#93a1a1:#fdf6e3"
        background_color = "#002b36"
        background_image = None
        cursor_color = "#eee8d5"
        foreground_color = "#839496"
    [[solarized-light]]
        palette = "#073642:#dc322f:#859900:#b58900:#268bd2:#d33682:#2aa198:#eee8d5:#002b36:#cb4b16:#586e75:#657b83:#839496:#6c71c4:#93a1a1:#fdf6e3"
        background_color = "#fdf6e3"
        background_image = None
        cursor_color = "#002b36"
        foreground_color = "#657b83"
[layouts]
    [[default]]
        [[[child1]]]
            type = Terminal
            parent = window0
            profile = default
        [[[window0]]]
            type = Window
            parent = ""
[plugins]




