## motion

```
sudo apt-get update
sudo apt-get upgrade -y
sudo apt-get install motion
```


```
sudo nano /etc/motion/motion.conf
```

```
daemon on  # 后台

width 640    # 像素宽
height 480   # 像素高

framerate 100  # 帧速率 减小延时

stream-localhost off #仅本机访问

ffmpeg_output_movies off #保存视频
```

```
sudo motion  # 启动
sudo service motion stop # 停止
```

pi-host:8081
