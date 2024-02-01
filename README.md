# 快速提取字体子集

## 环境准备

### 安装 Python

- 进入[官网](https://www.python.org/)，根据 32 位 windows 操作系统还是 64 位 windows 操作系统下载对应安装文件[Download Windows x86-64 executable installer](https://www.python.org/ftp/python/3.8.6/python-3.8.6-amd64.exe)

- 查看是否安装成功

```
python -V
// 显示Python 3.18.6

pip -V
// 显示pip 20.2.1
```

### 修改 pip 镜像源

- 路径： 在文件夹地址栏中输入 %APPDATA%
- 创建 pip.ini 文件

```
[global]

index-url=https://pypi.tuna.tsinghua.edu.cn/simple

[install]

use-mirrors=true

mirrors=https://pypi.tuna.tsinghua.edu.cn/simple

trusted-host=pypi.tuna.tsinghua.edu.cn
```

### 将 Python、pip 执行程序加入到 win10 系统环境 path 变量中

### VScode 安装 Python、Jupyter 插件

打开命令提示符安装依赖

```
pip install ipykernel -U --user --force-reinstall

pip install fontTools
```

### 启动

- 打开`characterSetExtraction.ipynb`文件

- 点击右上方选择内核，选择安装好的 Python 应用程序

- `characterSet.txt`添加需要提取的字体

- 点击全部运行
