# PyTorch + Visdom 安装配置指南（Windows）

> 适用于 Anaconda 用户，解决 Visdom 蓝屏、前端资源加载失败等问题。

#先启动pytorch环境
conda activate pytorch

#下载visdom
pip install visdom

#地址一般在
ANACONDA3\envs\pytorch\Lib\site-packages\visdom\server\run_server.py

#打开此py文件后 ctrl+F查找def def download_scripts_and_run():
注释掉download_scripts()
![alt text](image.png)

再将visdom\static删除将新的static文件复制进去

#再激活visdom
在pytorch环境输入visdom即可
