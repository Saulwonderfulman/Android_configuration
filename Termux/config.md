1 隐藏后台卡片

2 软件安装
pkg vim yazi syncthing

3 yazi配置
  安装字体
  1.创建Termux配置目录
  mkdir -p ~/.termux
2.下载字体
cd ~/.termux
wget https://github.com/ryanoasis/nerd-fonts/releases/latest/download/JetBrainsMono.zip
3.解压并移动字体
unzip JetBrainsMono.zip
mv JetBrainsMono-Regular.ttf ~/.termux/font.ttf
4.重新加载Termux配置
termux-reload-settings
