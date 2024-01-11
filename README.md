[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)

新教学 Wiki （2024）的全部源代码，基于 [mkdocs](http://www.mkdocs.org/) 。

本项目的部分代码正常检出需要预先安装和配置好 [git-lfs](https://github.com/git-lfs/git-lfs/wiki/Installation) 。

本地构建和运行站点方法如下：

```bash
# 一次获取所有文件（包括 GIT-LFS 管理的文件和所有子模块管理的文件）
# 目前 docs/courses 目录大小超过 650 MB
# 本方法的 clone 耗时可能较长
git clone https://github.com/c4pr1c3/cuc-wiki.git --recursive

# （可选）不获取所有 GIT-LFS 管理的文件和所有子模块管理的文件
GIT_LFS_SKIP_SMUDGE=1 git clone https://github.com/c4pr1c3/cuc-wiki.git

# （可选）单独下载 GIT-LFS 管理文件
git lfs pull

cd cuc-wiki 

# （可选）单独更新子模块
git submodule init && git submodule update

# 安装 mkdocs 相关的依赖
pip install mkdocs mkdocs-material pygments

# 使用 mkdocs 内置服务器提供本机可访问网站服务： http://127.0.0.1:8000/
mkdocs serve

```

