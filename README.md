# aclivechat
用于OBS仿YouTube风格的AcFun直播评论栏

![XSplit截图](https://raw.githubusercontent.com/ShigemoriHakura/aclivechat/master/screenshots/xsplit.png)  
![OBS截图](https://raw.githubusercontent.com/ShigemoriHakura/aclivechat/master/screenshots/obs.png)  

## 感谢：
* 前端来自： https://github.com/xfgryujk/blivechat
* 后端弹幕获取： https://github.com/orzogc/acfundanmu

## 使用
* 运行aclivechat.exe
* 浏览器打开：[http://localhost:12451](http://localhost:12451)

**注意事项：**

* 应该先启动livechat后启动OBS，否则网页会加载失败，失败时应刷新OBS的浏览器源，显示Loaded则加载成功
* 本地使用时不要关闭livechat.exe，否则不能继续获取弹幕
* 样式生成器没有列出所有本地字体，可以手动输入本地字体
* 房间号就是UID

### 从源代码编译
1. 编译前端（需要安装Node.js和npm【或者用cnpm更快】）：
   ```sh
   cd frontend
   npm i 【cnpm i】
   npm run build
   ```
   
2. 编译后端（需要安装go）
   ```sh
   go build
   ```
   
3. 正确放置文件
   ```sh
   前端 /dist
   后端 /
   ```

4. 浏览器打开[http://localhost:12451](http://localhost:12451)