# deepinwine-arch
打包了deepin上的wine qq,tim以及所需依赖到archlinux 上

pkg.tar.xz是打包好的，文件夹里的都是PKGBUILD（有时间传AUR上去）

其次安装deepin-wine，用sudo pacman -U安装
其中deepin-wine deepin-wine32 deepin-wine-helper deepin-fonts-wine deepin-libwine deepin-wine-uninstaller deepin-udis86都是要的
udis86不要用AUR里的那个，这里已经给出安装包

然后选择qq或tim（可以都装）安装

对于2k高分屏如需进行缩放：WINEPREFIX=~/.deepinwine/Deepin-QQ deepin-wine winecfg
在Graphics里改成120dpi

可以记录密码，运行效果和deepin上一样，稳定性还是可以的

(重要)如果使用TIM经常用一会就闪退的话，因该是~/.deepinwine/Deepin-TIM/drive_c/windows/system32/msls31.dll这东西的锅，据说bug已经修复了。。。还是有问题的话就从网上下个msls31.dll然后覆盖掉
