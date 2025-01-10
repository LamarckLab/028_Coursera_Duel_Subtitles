# 028_Coursera_Duel_Subtitles

这段前端JS代码用于临时添加Coursera的双字幕

```Javascript
var myvideo = document.getElementsByTagName('video')[0];
for (var i = 0; i < myvideo.textTracks.length; i++) {
    ["en", "zh-CN"].indexOf(myvideo.textTracks[i].language) > -1 ? myvideo.textTracks[i].mode = "showing" : myvideo.textTracks[i].mode = "hidden";
}
```
