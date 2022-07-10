# Pass-xueanquan
快速完成安全教育平台(xueanquan.com)作业的js代码

### 使用方法
- 打开作业页面
- 按下`F12`打开devTool
- 切换到Console(控制台)选项
- 粘贴代码回车

### 安全学习(看视频作题)
```js
try {
    ShowTestPaper();
    var radios = document.getElementsByTagName("input");
    for (let i = 0; i < radios.length; i++) {
        const r = radios[i];
        r.checked = r.value == 1 ? true : false;
    }
    document.getElementById("input_button").click();
} catch (error) {}
```
### 专题活动(活动二问卷)
```
try {
    var radios = document.getElementsByTagName("input");
    for (let i = 0; i < radios.length; i++) {
        radios[i].click();
    }
} catch (error) {}
```

### 专题活动(互动视频)
```js
var starts = document.getElementsByClassName("img1");
for (let i = 0; i < starts.length; i++) {
    const s = starts[i];
    s.click();
}
setInterval(() => {
    var videos = document.getElementsByTagName("video");
    for (let i = 0; i < videos.length; i++) {
        const v = videos[i];
        try {
            v.currentTime = v.duration + 1;
        } catch{}
    }
}, (1000));
```
