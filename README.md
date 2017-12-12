# boilerplate

## chrome 拓展可以做什么？

## 基本

可以有四个地方执行代码

- tab   (main.html)
- popup     (popup.html)
- options   (options.html)
- content   (background.js)

### tab

可以覆盖 new tab:

```
"chrome_url_overrides": {
  "newtab": "main.html"
},
```

### popup

点击图标出现的内容区。


### options

右键图标 -> 选项 跳转的页面，主要是配置该拓展。

### content

在页面中执行代码，配置在每个页面都执行。

## 结构


## 魔改

```bash
~/Library/Application Support/Google/Chrome/Default/Extensions
```
存放了安装的`chrome`拓展，找到对应的`id`即可，但可惜大部分拓展都是压缩后的。

