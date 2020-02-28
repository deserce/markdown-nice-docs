## 环境

- [Node.js](https://www.runoob.com/nodejs/nodejs-tutorial.html) v10.13.0
- [yarn](https://yarnpkg.com/lang/zh-hans/docs/) v1.12.3

## 开发流程

下载项目、切换目录、安装依赖包和开始运行

```shell
$ git clone git@github.com:mdnice/markdown-nice.git
$ cd markdown-nice
$ yarn
$ yarn start
```

运行后即可在浏览器中访问 `http://localhost:3000` 可看到页面

## 组件调试

目前使用 storybook 做组件调试

```shell
$ yarn storybook
```

## 主要开发库

- [React](https://github.com/facebook/react "React")：facebook 开源的 js 视图层框架
- [markdown-it](https://github.com/markdown-it/markdown-it "markdown-it")：markdown 转换富文本解析器
- [juice](https://github.com/Automattic/juice "juice")：将 CSS 类选择器转换为行内样式的工具
- [codemirror](https://github.com/codemirror/codemirror "codemirror")：网页代码编辑器
- [ant-design](https://github.com/ant-design/ant-design "ant-design")：React UI组件库
- [mobx](https://github.com/mobxjs/mobx "mobx")：状态管理库
- [highlight.js](https://github.com/highlightjs/highlight.js "highlight.js")：代码高亮库
- [MathJax](https://github.com/mathjax/MathJax "MathJax-node")：公式转图片库
- axios、ali-oss、qiniu-js等

## 目录结构

```shell
├── README.md                   // 项目说明
├── package.json                // 依赖包
├── watch.js                    // 监听组件变化
└── src                         // 源代码
    ├── component               // 组件            
    ├── icon                    // 图表                 
    ├── layout                  // 布局
    ├── store                   // 状态管理
    ├── template                // 模板
    │   ├── code                // 代码样式
    │   ├── markdown            // 主题样式
    │   ├── basic.js            // 基础样式
    │   └── content.js          // 示例文章
    ├── utils                   // 通用库
    └── App.js                  // 入口
```