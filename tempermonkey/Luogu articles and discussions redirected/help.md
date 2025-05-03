# 帮助指南
## 介绍&使用方法
tempermonkey插件：在页面左下角添加一个蓝色按钮，点击后：当访问https://www.luogu.com.cn/article/xxxxxx或者https://www.luogu.com/article/xxxxxx的时候跳转到https://www.luogu.me/article/xxxxxx，当访问https://www.luogu.com.cn/discuss/yyyyyy或者https://www.luogu.com/discuss/yyyyyy的时候跳转到https://lglg.top/yyyyyy。  
左下角会出现“快速跳转”蓝色按钮。
## 安装地址
网络剪贴板： https://netcut.cn/luogu-chajian-100000  
或者此处(github)。

安装方法：  
1.确保已安装Tampermonkey扩展

2.点击Tampermonkey图标，选择"创建新脚本"

3.删除默认内容，粘贴上面的代码

4.保存脚本(Ctrl+S)
## 功能说明
这个脚本会在页面左下角添加一个蓝色的"快速跳转"按钮

当点击按钮时，会根据当前URL执行以下操作：

如果是文章页面（包含/article/），会跳转到https://www.luogu.me/article/xxxxxx。

如果是讨论页面（包含/discuss/），会跳转到https://lglg.top/yyyyyy。

按钮有悬停效果，鼠标悬停时会变深蓝色。
## 注意
脚本只会在匹配的URL（洛谷文章和讨论页面）上运行。
