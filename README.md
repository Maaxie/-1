# -1
https://mp.weixin.qq.com/s?__biz=MzI4MzAwNTQ3NQ==&mid=209866190&idx=1&sn=0ee75509eb2fab454009125e0a8c6437&scene=0#rd


# docker run -d \
  -v /etc/localtime:/etc/localtime:ro \
  -v /tmp/.X11-unix:/tmp/.X11-unix \
  -e DISPLAY=unix$DISPLAY \
  -v $HOME/slides:/root/slides \
  -e GDK_SCALE \
  -e GDK_DPI_SCALE \
  --name libreoffice \
  jess/libreoffice


开启docker图形话界面时候的指令，主要是：
nvidia-docker run  --shm-size=8gb   -it -v `pwd`:/workspace -e DISPLAY=unix$DISPLAY -v /tmp/.X11-unix:/tmp/.X11-unix 1240803839cgw/cuda_caffe:latest
开机需要执行 xhost +
