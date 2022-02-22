# Koishi 模板仓库

- [安装方法](#安装方法)
  - [从当前仓库创建](#从当前仓库创建)
  - [使用包管理器创建](#使用包管理器创建)
- [基本功能](#基本功能)
  - [启动机器人](#启动机器人)
  - [设置环境变量](#设置环境变量)
  - [工作区开发](#工作区开发)

## 安装方法

我们提供了两种安装方法。你可以使用其中的任意一种。

### 从当前仓库创建

1. 点击 [**这里**](https://github.com/koishijs/boilerplate/generate) 以创建此仓库的副本。<br>注意：这是一个模板仓库，创建副本不同于 fork，它生成的新仓库不会包含当前仓库的提交历史。
2. 将你创建的项目 clone 到本地，并在本地目录启动命令行。
3. 输入 `npm install` / `yarn` 安装依赖。
4. 输入 `npm run dev` / `yarn dev` 开始运行。

### 使用包管理器创建

在任意目录启动命令行，输入下面的指令：

```sh
npm init koishi         # yarn create koishi
```

跟随提示即可完成安装流程。

由于国内可能无法访问 GitHub，你可能需要科学上网或使用镜像。下面提供一种使用镜像的写法：

```sh
npm init koishi -m https://hub.fastgit.xyz
```

## 基本功能

### 启动机器人

在机器人的目录下输入下面的命令行即可启用机器人：

```sh
# 开发模式
npm run dev             # yarn dev

# 生产模式
npm start               # yarn start
```

如果你不进行工作区开发，那么开发模式和生产模式将几乎没有区别。

### 设置环境变量

你可以在当前目录创建一个 `.env` 文件，并在里面填写你的环境变量。这个文件已经被包含在 `.gitignore` 中，你可以在其中填写隐私信息（例如账号密码）而不用担心被上传到远端。参见 [**dotenv**](https://github.com/motdotla/dotenv)。

### 工作区开发

除了上面介绍的用法以外，我们还提供了更多功能：

- build：构建源代码
- bump：更新版本号
- init：创建新插件
- pub：发布插件

具体用法请参考 [**官方文档**](https://koishi.js.org/guide/introduction/workspace.html)。
