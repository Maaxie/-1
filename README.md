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


# 错误
Gtk-Message: Failed to load module "canberra-gtk-module"
libGL error: No matching fbConfigs or visuals found
libGL error: failed to load driver: swrast
The program 'Depth' received an X Window System error.
This probably reflects a bug in the program.
The error was 'BadValue (integer parameter out of range for operation)'.
  (Details: serial 51 error_code 2 request_code 154 minor_code 3)
  (Note to programmers: normally, X errors are reported asynchronously;
   that is, you will receive the error a while after causing it.
   To debug your program, run it with the --sync command line
   option to change this behavior. You can then get a meaningful
   backtrace from your debugger if you break on the gdk_x_error() function.)


