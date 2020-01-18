# My fonts collections
收集的一些适合编程的字体，放到GitHub上方便以后自己下载, 请按自己喜好安装使用.

下面以 `YaHei Consolas Hybrid 1.12`为例

## 安装
clone下来
```
git clone https://github.com/leoatchina/fonts-collection.git
```

## vim里使用
在配置文件里加入下面这行, 11.5是字体大小
```
set guifont=YaHei\ Consolas\ Hybrid\ 11.5
```

## windows
在字体文件上点右键,安装

## osx
双击字体安装

## linux
 在/usr/share/fonts/truetype/, 下建立一个新的目录 YaHei\ Consolas\ Hybrid
```
sudo mkdir -p /usr/share/fonts/truetype/YaHei\ Consolas\ Hybrid
```
 将YaHei Consolas Hybrid 1.12.ttf 复制到刚才建立的文件夹里.
```
sudo cp YaHei\ Consolas\ Hybrid\ 1.12.ttf /usr/share/fonts/truetype/YaHei\ Consolas\ Hybrid
```
 修改字体文件的权限.
```
cd /usr/share/fonts/truetype/YaHei\ Consolas\ Hybrid
sudo chmod 644 YaHei\ Consolas\ Hybrid\ 1.12.ttf
```
开始安装字体.
```
sudo mkfontscale
# 创建字体的fonts.scale文件，它用来控制字体旋转缩放
sudo mkfontdir
# 创建字体的fonts.dir文件，它用来控制字体粗斜体产生
sudo fc-cache -fv
# 建立字体缓存信息，也就是让系统认识该字体
```
