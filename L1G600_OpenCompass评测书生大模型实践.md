## 1、首先跑通大模型api的评测代码
首先安装环境，按文档安装但是出现问题，第一次提示importlib_metadata没有安装，查看pip list确实没有这个库并手动安装。
接下来又提示没有安装rouge库，但是pip list中有这个库，手动卸载pip uninstall rouge,再尝试手动安装 pip install rouge后成功。
![image](https://github.com/user-attachments/assets/ae16ba4f-5d49-456b-8ca7-5ffe9d971478)

## 2、跑本地大模型的评测代码
首先安装环境，执行测试代码确认安装成功。(最浪费时间的就是装库配置环境)
![image](https://github.com/user-attachments/assets/33b24661-41f1-4072-b4d0-1c05fb91d28b)
又报错了
ValueError: numpy.dtype size changed, may indicate binary incompatibility. Expected 96 from C header, got 88 from PyObject
通过重装torch，解决。
运行代码，成功
![image](https://github.com/user-attachments/assets/f2080c5a-c88e-4d0b-b334-2b1b9809eb47)
