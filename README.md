
## 砚台主题-gruvbox

这是一个砚台（Inkstone）的示例主题（[https://github.com/2061360308/InkStone-Markdown/](https://github.com/2061360308/InkStone-Markdown)）

> 砚台的主题功能还处于开发阶段，截至目前`V0.3.2`版本还为提供该功能，你可以在仓库的develop分支找到支持此功能的最新开发版本（develop分支被部署在[https://dev.inkstone.work](https://dev.inkstone.work)）

## 主题使用

请在[`release`](https://github.com/2061360308/inkstone-theme-gruvbox/releases/latest)页面下载最新的资源文件（gruvbox.zip）。进入砚台设置面板，基础设置>主题>加载本地主题。弹出文件选择框中选择之前下载的gruvbox.zip，再看到主题加载成功提示后则证明新主题已经安装成功。你可以再主题设置的下拉选项菜单中找到并选用该主题。

如果不需要某个主题时只需要在设置中找到该主题，鼠标悬浮可以看到对应的删除按钮，单击删除在弹出确认框中确认即可删除。

## 主题开发

砚台主题包就是资源文件的zip压缩包，所有资源文件中最重要的是`theme.json`文件，请确保它为以下格式

```json
{
  "name": "gruvbox", // 主题名，必须
  "version": "1.0.0",  // 版本号，必须
  "author": "盧瞳",  // 作者名，必须
  "url": "url",  // 主题发布的GitHub仓库url，必须
  "mainCss": "theme.css",  // 主题css文件，必须
  "highlightTheme": "base16/gruvbox-light-soft",  // Vditor编辑器中highlight.js主题亮色样式，可选
  "highlightDarkTheme": "base16/gruvbox-dark-soft",  // Vditor编辑器中highlight.js主题暗色样式，可选
  "codeMirrorTheme": "light.js",  // Codemirror编辑器中主题需要的亮色样式，可选
  "codeMirrorDarkTheme": "dark.js"  // Codemirror编辑器中主题需要的暗色样式，可选
}
```

补充：

1. **theme.css** ：用于设计自定义的css样式，你可以在inkstone中点击F12打开开发者面板获取对应元素class名
2. **highlightTheme**/**highlightDarkTheme** ：highlightjs中所有支持的主题可在[highlightjs 官方](https://github.com/highlightjs/highlight.js/tree/main/src/styles)中找到
3. **codeMirrorTheme**/**codeMirrorDarkTheme** ： codemirror6需要使用Javascript创建自定义主题，有关更多主题的示例可以查看[craftzdog/cm6-themes](https://github.com/craftzdog/cm6-themes)

> 你可以使用scss、typescript等工具协助开发，目前由于该功能开发不完善还没有相关示例

## 参考资源

inkstone-theme-gruvbox 使用Gruvbox主题相关资源参考了以下内容：

[YV31/gruvbox-css](https://github.com/YV31/gruvbox-css)

[highlightjs](https://github.com/highlightjs/highlight.js/tree/main/src/styles)

[craftzdog/cm6-themes](https://github.com/craftzdog/cm6-themes)
