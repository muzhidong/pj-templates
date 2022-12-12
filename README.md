# 原生微信小程序项目模板
## 特性
- 提供模块引入统一入口

	在`app/module`文件中通过`export ... from ...`语法糖引入所有模块，统一入口，有利于代码维护。

- 支持使用Sass编写样式

	利用Sass特性，封装主题色变量、常用混入如iPhoneX刘海兼容、函数如rpx2percent等，提升开发效率和项目可维护。
	
	`npm run start`启动gulp脚本，对全局样式文件、页面局部样式文件自动生成对应的scss文件，并监听其变化，自动编译写入到wxss，方便开发者实时查看效果。

- 支持开发环境一键切换

	使用小程序的非正式版，每次冷启动小程序，会弹出Action Sheet，供用户切换使用的环境，大大提升开发或QA的工作效率。

- 提供常用behaviors

	如订阅、分享(转发)、埋点、广告等。

- 提供常用正则

	如身份证、邮箱、手机号、中文名等

- 提供常用工具

	如节流防抖、或有关存储、时间、金钱、请求、监控、表情符号等工具

- 支持代码分析&图片压缩

	通过引入`miniprogram-slim`工具实现

## 模板选择
- 分支`tpl-sass`

	没有分包结构的小程序模板

- 分支`tpl-subpackage-sass`

	有分包结构的小程序模板
