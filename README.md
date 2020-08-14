# AKFun 前端脚手架

> AKFun 是一个基于 Webpack4.0 的打包工具，支持多种技术栈：Vue技术栈、React技术栈、React&TS技术栈(开发中)
- 技术栈：node/webpack4.0/express/babel/eslint/stylelint

## 特性
- ⚡️ 零配置，开箱即用
- 👏 支持Vue和React项目的构建
- 📤 支持单页面和多页面
- 💪 提供三种构建场景: 本地开发调试模式(包含热更新、接口代理等功能)、构建生产环境代码、library库的构建
- ❤️ 开放配置能力: 可配置构建入口文件、是否开启ESLint代码规范检测、resolve和externals配置、接口代理配置等
- 👍 支持 [Sass](https://sass-lang.com/)、[PostCSS](https://postcss.org/)、[ESLint](http://eslint.cn/)、[StyleLint](https://github.com/stylelint)
- 😀 提供完整的Vue和React项目模板


## 使用方法一（使用AKFun创建一个新项目）：全局安装使用AKFun
> 可用于同时管理多个前端项目代码

1. **全局安装**

```bash
# 安装
$ npm i -g akfun 或者 yarn add akfun global
```

2. **初始化一个项目**
> 可选择项目类型：vue或者react，默认react类型的项目，也可通过--dir参数指定存放项目模板的目录
```bash
$ akfun init -t=vue
```

3. **开始使用：以全局命令方式构建项目（确保已yarn install或者npm install）**

```bash
# 1、开启本地调试模式
$ akfun dev
```

```bash
# 2、构建生产环境代码
$ akfun build
```

```bash
# 3、构建第三方功能包
$ akfun build2lib
```

## 使用方法二（现有项目赋予AKFun的前端工程能力）
> 在现有项目中局部安装AKFun

1. **本地安装**

```bash
$ npm i akfun --save-dev 或者 yarn add akfun --dev
```

2. **在package.json中创建可执行脚本**
> 打开package.json，在scripts中新增三条可执行命令

```bash
# 用于开启本地调试模式
"dev": "akfun dev"
# 用于构建生产环境代码
"build": "akfun build"
# 用于构建第三方功能包
"build2lib": "akfun build2lib"
```

3. **开始构建当前项目**

# 开启本地调试模式
```bash
$ npm run dev
```

# 构建生产环境代码
```bash
$ npm run build
```

# 构建第三方功能包
```bash
$ npm run build2lib
```

## 使用注意事项
1. akfun的默认构建入口文件: ./src/index.js
2. 根目录下的akfun.config.js为当前项目的配置文件，优先级最高（可覆盖AKFun提供的默认配置）
3. 多页面场景: 当



