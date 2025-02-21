# 简介

> Free software, open standards, and web services for interactive computing across all programming languages.

https://jupyter.org/

https://ipython.readthedocs.io/en/stable/index.html



# 安装

1、安装`Anaconda`或者`Miniconda`



```shell
# conda安装jupyter

# 创建新的虚拟环境
conda create -n my_env python=3.8 scikit-image=0.18 -y
# 查看新环境是否已经创建成功
conda env list

# 进入新创建的环境
conda activate my_env
# 安装Jupyter
pip install jupyter

# 新建一个notebook并且使用当前新建的环境时，发现没有当前新建环境的IPython内核。
# 在当前环境下建立新的IPython内核后，再次启动jupyter notebook发现已经有了当前环境下的IPython内核

# 在当前环境下建立新的IPython内核
# 安装ipykernel
pip install ipykernel
# 生成ipykernel的配置文件
python -m ipykernel install --name env_name
# 查看已有的kernel
jupyter kernelspec list
```





```shell
# 查看配置选项
jupyter notebook -h
jupyter notebook --help

配置文件配置

# 生成配置文件
jupyter notebook --generate-config
# 配置文件的位置
~/.jupyter                    # linux系统
C:\Users\<UserName>\.jupyter  # windows系统
# 配置文件，jupyter_notebook_config.py

# 在浏览器中自动打开notebook
jupyter notebook
```



# 快捷键



# 扩展

`A collection of various notebook extensions for Jupyter`

https://github.com/ipython-contrib/jupyter_contrib_nbextensions.git

扩展文档

https://jupyter-contrib-nbextensions.readthedocs.io/en/latest/

```shell
# 安装扩展包
pip install jupyter_contrib_nbextensions
# 安装 javascript和css文件
jupyter contrib nbextension install --user

# 启动juputer notebook，发现多了Nbextensions
```

几个比较有用的扩展

```
variable inspector
table of content
snippets
codefolding
autopep8
hide input
split cell notebook
zenmode
```



# 参考

https://blog.csdn.net/qq_40918859/article/details/125067935

https://blog.csdn.net/cainiao_python/article/details/125567913



https://www.bilibili.com/video/BV1Q4411H7fJ/?share_source=copy_web

