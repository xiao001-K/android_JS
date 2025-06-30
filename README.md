# android_JS 介绍
基于linsheng_FATJS开源二次修改优化

>>>FATJS 基于安卓无障碍的自动化框架｜集成找色模块｜引入JS引擎｜Api类似Autojs


```js
//双击点赞
const minX = 400;  
const maxX = 500;  
const minY = 700;  
const maxY = 800; 
var x = Math.floor(Math.random() * (maxX - minX + 1)) + minX;  
var y = Math.floor(Math.random() * (maxY - minY + 1)) + minY;  
doubleClick(x,y);
//设置剪切板内容并打印
clip('剪贴板文本');
let clipboardText = getClip();
if (clipboardText) {
    print("剪贴板内容: " + clipboardText);
} else {
    print("剪贴板为空或无法获取内容");
}

//打开悬浮窗
showLog() 
print('返回桌面') //打印日志
home()
print('点击设置')
text('设置').findOne().click()
sleep(2000) //等待2s
back() //返回
hideLog() //隐藏悬浮窗
click(100, 200) // 点击坐标
capture('/sdcard/1.png') // 截屏
...
