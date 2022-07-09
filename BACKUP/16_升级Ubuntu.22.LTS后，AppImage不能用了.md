# [升级Ubuntu 22 LTS后，AppImage不能用了](https://github.com/gnimg/gitblog/issues/16)

升级Ubuntu 22.04 LTS后，一切都非常的顺利，但是突然发现，AppImage封装的程序都不能用了。出现了与Fuse相关的问题。

`Failed to load libfuse.so.2`

问题在于，当你尝试去安装fuse2的时候，系统会提示，Fuse3已经安装了。

解决办法：只需要安装`libfuse-dev`库。就可以。

```bash
sudo apt-get install libfuse-dev
```
