# mmPlayer V1.2.1（2018.03.01）
模仿QQ音乐网页版界面，采用flexbox和position布局；
mmPlayer虽然是响应式，但主要以为PC端为主，移动端只做相应适配（未做歌词显示）

> api：一个开源的[网易云音乐 NodeJS 版 API](https://binaryify.github.io/NeteaseCloudMusicApi)（有api才有动力写！！！）

> [在线演示地址](http://music.mtnhao.com)

## 安装与使用

> 后台服务器

```
cd mmPlayer/server

npm install //安装依赖

node app.js //服务端运行 访问 http://localhost:3000
```

> mmPlayer

```
git clone https://github.com/maomao1996/mmPlayer.git  //下载mmPlayer

cd mmPlayer

npm install //安装依赖

npm run dev //服务端运行

npm run build  //项目打包
```
需要修改api目录下music的url地址为后台服务器地址

## 技术栈

- Vue（核心框架）
- Vue-Router（页面路由）
- Vuex（状态管理）
- axios（网络请求）

## 功能

- 播放器
- 歌词滚动
- 排行榜
- 搜索
- 播放历史

## 界面欣赏

![正在播放](http://img.mukewang.com/5a781eb10001d47c19201004.png)
![排行榜](http://img.mukewang.com/5a781cdf000125ad19201004.png)

## 更新说明
### V0.1.0（2018.01.24）
- 发布试用版

### V0.2.0（2018.01.29）
- 新增音量控制模块
- 优化歌曲选中

### V1.0.0（2018.02.05）
- 发布正式版（因为一系列原因，mmPlayer V1.0.0版本在试用版的基础上进行了重构了，并引入了Vue-Router和Vuex
- 当前播放歌曲高亮（感觉一个小GIF还不够）
- 优化快速切歌导致歌曲播放失败的问题
- 进度条拖动适配移动端
- 优化点击时可能出现的半透明背景
- 新增排行榜

### V1.1.0（2018.02.09）
- 新增我听过的（播放历史）
- 整合公用列表组件
- 新增mmToast插件
- 整合字体大小、颜色相关CSS
- 优化清空正在播放列表功能

### V1.2.0（2018.02.28）
- 新增搜索功能
- 新增歌曲删除功能（正在播放列表和播放历史列表中）
- 使用ES6的class对数据进行二次处理
- 优化歌词居中显示
- 优化播放可能出现的错误
- 因部分问题，去除清空正在播放列表功能

### V1.2.1（2018.03.01）
- 优化正在播放列表第一次加载
- 优化删除歌曲
- 优化Vuex模块
- 优化加载loading
- 优化移动端适配
- 提高代码复用性

## 后续功能
- 歌手
- 热门歌单
- 收藏
- 同步网易云歌单

## 其他说明

- 个人练手项目
- 预计后续将发布小程序版本

