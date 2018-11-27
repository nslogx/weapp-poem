### 诗词墨客
本仓库是诗词墨客小程序对应的开源仓库，旨在分享微信小程序的开发经验。

该项目采用 [Wepy](https://github.com/wepyjs/wepy) 框架 + [iview-weapp](https://github.com/TalkingData/iview-weapp) UI组件库，古诗词数据源来自于 [chinese-poetry](https://github.com/chinese-poetry/chinese-poetry) 开源仓库，包含5.5万首唐诗、26万首宋诗和2.1万首宋词. 唐宋两朝近1.4万古诗人, 和两宋时期1.5K词人。

感谢相关作者的努力及开源精神。

### 使用

``` bash
git clone git@github.com:huangjianke/weapp-poem.git
cd weapp-poem
npm install wepy-cli -g
npm install
wepy build --watch
```

- 使用微信开发者工具新建项目，本地开发**选择 `dist` 目录**
- 微信开发者工具 -> 项目
  - **关闭** ES6 转 ES5
  - **关闭** 代码压缩上传
  - **关闭** 上传代码时样式文件自动补全
  - **开启** 开发环境不校验请求域名、TLS版本以及HTTPS证书

[Wepy](https://github.com/wepyjs/wepy) 具体使用可参考：[WePY项目的创建与使用](https://tencent.github.io/wepy/document.html#/?id=wepy%E9%A1%B9%E7%9B%AE%E7%9A%84%E5%88%9B%E5%BB%BA%E4%B8%8E%E4%BD%BF%E7%94%A8)

古诗词数据存储于 [LeanCloud](https://leancloud.cn/)，使用前先在[LeanCloud](https://leancloud.cn/) 注册App，然后导入由 [chinese-poetry-mysql](https://github.com/KomaBeyond/chinese-poetry-mysql) 整理的 mysql 格式数据，并在 `app.wpy` 中配置您自己的App相关信息

### 扫码体验

扫码访问小程序:

![诗词墨客](https://raw.githubusercontent.com/huangjianke/weapp-poem/master/images/code.png)

## 部分页面展示
|摘录|详情|
| :---: | :---: |
|![摘录](https://raw.githubusercontent.com/huangjianke/weapp-poem/master/images/img00.png) | ![详情](https://raw.githubusercontent.com/huangjianke/weapp-poem/master/images/img01.png)|
|文库|作者|
|![文库](https://raw.githubusercontent.com/huangjianke/weapp-poem/master/images/img02.png) | ![作者](https://raw.githubusercontent.com/huangjianke/weapp-poem/master/images/img03.png)|

### Todo

- [ ] 增加搜索功能
- [ ] 增加生成摘录卡片功能
- [ ] 增加收藏功能

### LICENSE

MIT License

Copyright (c) 2018 huangjianke

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
