# tinper-bee-components

> 获得所有组件，所有版本的示例文件

## 使用步骤

- server/createFile.js 文件中填写cdn配置
- npm run getTag  //获得所有组件的已有tag
- npm run createFile  //创建对应文件下的 demo.js 和 demo.css,并增量上传到cdn



## 注意：

- 要求组件git仓库必须有 dist目录，且dist目录中存在demo.js、demo.css
- 在下载demo时，有问题的组件库，写入 static/error.txt中， 目前已知 bee-complex-grid、bee-tooltip、bee-viewer部分tag有问题，没有dist目录
- 如需要重新获取组件tag文件，删除 components目录，执行 `npm run getTag && npm run createFile` 后，手动上传到 cdn