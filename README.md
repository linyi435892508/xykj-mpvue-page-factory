README
===========================
解决mpvue多个页面公用一个vm对象的问题 [mpvue issue 140](https://github.com/Meituan-Dianping/mpvue/issues/140)

### 使用方法:

pagckage.json 中添加依赖
```
"mpvue-loader": "git+https://github.com/linyi435892508/xykj-mpvue-load.git",
"mpvue-page-factory": "^1.0.1",
```

#### 添加完依赖以后，需要修改页面的main.js入口文件为
 ```javascript
import pageFactory from 'mpvue-page-factory'
import App from './index'

Page(pageFactory(App))
```
