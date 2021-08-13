# `Java` 项目开发指南

[![publish](https://github.com/lwpk110/tendata-javadoc/actions/workflows/gh-pages.yml/badge.svg)](https://github.com/lwpk110/tendata-javadoc/actions/workflows/gh-pages.yml)
![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/lwpk110/tendata-javadoc)
![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/lwpk110/tendata-javadoc)
## 本地运行

**环境要求：**

- python： 3.0+

### 1. 克隆项目

```bash
git clone https://github.com/lwpk110/tendata-javadoc.git
```

### 2. 初始化环境

项目预览需要安装 Python 环境来启动 server，强烈建议使用 Python 3.6+ 的版本。如果本地没有 Python 环境，也可以使用 [Docker预览服务器](https://squidfunk.github.io/mkdocs-material/creating-your-site/#creating-your-site) 来启动。

#### 2.1 本地初始化

安装依赖

```bash
pip install -r requirements.txt
```

#### 2.2 使用 Docker 初始化

```bash
docker pull squidfunk/mkdocs-material
```

### 3. 预览

#### 3.1 本地预览

```bash
mkdocs serve
```

#### 3.2 使用 Docker 预览

**uinx**:

```bash
docker run --rm -it -p 8000:8000 -v ${PWD}:/docs squidfunk/mkdocs-material
```

**Windows**:

```bash
docker run --rm -it -p 8000:8000 -v "%cd%":/docs squidfunk/mkdocs-material
```

## 协作规范

文档使用 Markdown 编写，使用 [mkdocs](https://www.mkdocs.org/) 配合 [mkdocs-material](https://squidfunk.github.io/mkdocs-material-insiders/) 主题构建。

- form
- code
- pr
