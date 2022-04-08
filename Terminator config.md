## terminator 安装方法 
```bash
sudo apt-get install terminator
```
    
## 颜色配置
```bash
mkdir ~/.config/terminator
cd ~/.config/terminator
vim config

[global_config]
focus = system
[keybindings]
[layouts]
[[default]]
[[[child1]]]
parent = window0
type = Terminal
[[[window0]]]
parent = ""
type = Window
[plugins]
[profiles]
[[default]]
background_color = "#2e2e2d"
cursor_color = "#25C3DC"
foreground_color = "#f2f2f2"
palette = "#2c2c2c:#c62828:#558b2e:#f9a825:#1565c1:#6a1e9a:#00838f:#ffffff:#969694:#f15250:#86bd47:#f8e63a:#77b2f6:#b963c8:#25c3dc:#ffffff"
```
    
## 分屏快捷键
```bash
crtl+shift+e / crtl+shift+o 
```