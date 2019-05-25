# Raspi_26pinLCD
How to config a LCD TFT screen 

## 配置ros 并附带LCD屏幕驱动安装
[RikiRobot镜像](https://pan.baidu.com/s/1pzuB15q_sQrVq6PdNdAeRQ) 提取码：tfoa

镜像密码：123456

## 解压文件烧写镜像
[镜像烧写软件](https://pan.baidu.com/s/1Tv0wZr4wMLgVZI6nOLF1Qg) 提取码：z0ug

## LCD屏幕
这里我使用的是一块26Pin 3.5 寸的触摸屏。[触摸屏某宝链接](https://item.taobao.com/item.htm?id=521698312415&price=60&original_price=63&sourceType=item&sourceType=item&suid=b6fa9d3b-3438-4c9d-a875-5445272dc661&ut_sk=1.W%2BqANxN2jRgDACKeq0FEcprr_21646297_1558756681302.Copy.1&un=c2a7ab61da0f9f789eedd86203cf18d8&share_crt_v=1&sp_tk=77+lS3B2UVlkcmNwV3bvv6U=&cpp=1&shareurl=true&spm=a313p.22.2xi.1035727603172&short_name=h.eWF9tON&sm=365039&app=chrome)
大家可以自行选择屏幕，链接仅供参考。

## LDC屏幕配置
```Bash
cd /boot

sudo wget http://blog.lxx1.com/wp-content/uploads/2017/03/LCD-show-170309.tar.gz
```

```Bash
sudo tar xzvf /boot/LCD-show-170309.tar.gz

cd LCD-show/
#选择自己设备对应的驱动，我使用的是3.5寸触摸屏
sudo chmod +x LCD35-show

sudo ./LCD35-show 
```
  运行结束后屏幕系统会重启，重启后屏幕已经可以触摸显示，本人在测试时，官方镜像显示后触摸屏会失准,使用RikiRobot的镜像没有此问题。
