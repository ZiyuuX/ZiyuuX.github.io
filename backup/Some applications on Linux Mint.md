## Calibre

```shell
sudo apt install -y libxcb-cursor-dev
sudo -v && wget -nv -O- https://download.calibre-ebook.com/linux-installer.sh | sudo sh /dev/stdin
```

## Rime 拼音输入法

```shell
sudo apt install -y ibus-rime
# 安装之后，重启电脑于托盘位置设置
```

## Power Saver

TLP is a highly configurable power saving tool for laptops. There is a flatpak called TLP gui or something if you want to tweak the config graphically (never tried it myself), or you can edit the config file directly. The default settings should be fine though.

```shell
sudo apt install tlp tlp-rdw smartmontools
sudo systemctl enable --now tlp.serv
```
Then, reboot. You can check the current status of tlp with

```shell
sudo tlp-stat
```