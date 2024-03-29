# dwm - catppuccin theme

![dwm-desktop](https://github.com/gin-18/pictures/blob/master/readme/dwm/dwm-desktop.png?raw=true)

![dwm-nvim-alpha](https://github.com/gin-18/pictures/blob/master/readme/dwm/dwm-nvim-alpha.png?raw=true)

![dwm-nvim-code-firefox](https://github.com/gin-18/pictures/blob/master/readme/dwm/dwm-nvim-code-firefox.png?raw=true)

![dwm-yazi](https://github.com/gin-18/pictures/blob/master/readme/dwm/dwm-yazi.png?raw=true)

![dwm-btop](https://github.com/gin-18/pictures/blob/master/readme/dwm/dwm-btop.png?raw=true)

## 内容列表

* [依赖的软件包](#依赖的软件包)
* [安装](#安装)
* [说明](#说明)

## 依赖的软件包

```
feh

picom

i3lock

flameshot

alsa-util

xorg-xbacklight

ttf-firacode-nerd
```

## 安装

```sh
git clone https://github.com/gin-18/dwm.git --depth 1

sudo make clean install
```

## 说明

在 `scripts/dwm-wallpaper.sh` 脚本中修改 `壁纸目录`。

在 `scripts/screen-lock.sh` 脚本中修改 `锁屏壁纸`。

在 `dwm.c` 中的下面这个函数中修改启动脚本的路径。

```c
void
runAutostart(void) {
  system("cd ~/github/gin-18/dwm/scripts; ./autostart.sh &");
}
```

`MODKEY` 是 `Window` 键。

| 快捷键                   | 描述                            |
|--------------------------|---------------------------------|
| `MODKEY` `p`             | 打开 `dmenu`                    |
| `MODKEY` `Enter`         | 打开终端                        |
| `MODKEY` `b`             | 隐藏状态栏                      |
| `MODKEY` `j`             | 顺时针选择窗口                  |
| `MODKEY` `k`             | 逆时针选择窗口                  |
| `MODKEY` `h`             | 减少主窗口的大小                |
| `MODKEY` `l`             | 增加主窗口的大小                |
| `MODKEY` `e`             | 隐藏当前窗口                    |
| `MODKEY` `Shift` `e`     | 显示隐藏的窗口                  |
| `MODKEY` `c`             | 关闭当前窗口                    |
| `MODKEY` `f`             | 将当前窗口全屏                  |
| `MODKEY` `F1`            | 减少屏幕亮度                    |
| `MODKEY` `F2`            | 增加屏幕亮度                    |
| `MODKEY` `F4`            | 静音                            |
| `MODKEY` `F5`            | 降低声音                        |
| `MODKEY` `F6`            | 增加声音                        |
| `MODKEY` `1 ~ 5`         | 切换到 `1 ~ 5` 标签下           |
| `MODKEY` `Shift` `1 ~ 9` | 将当前窗口移动到 `1 ~ 5` 标签下 |
| `MODKEY` `Shift` `Enter` | 将当前窗口提升为主窗口          |
| `MODKEY` `Shift` `q`     | 退出 `dwm`                      |
| `MODKEY` `Shift` `l`     | 锁屏                            |
| `MODKEY` `Shift` `w`     | 切换壁纸                        |
| `MODKEY` `Shift` `s`     | `flameshot` 截图                |
