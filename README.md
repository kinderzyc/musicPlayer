# musicPlayer

### 音乐API
---
属性
```
audioObject 创建或者获取audio对象
audioObject.play() //开始播放
audioObject.pause() //暂停播放
audioObject.autoPlay = true


//设置或者获取自动播方状态，默认为false不自动播放
audioObject.src //设置或者获取音乐地址
audioObject.volume //设置或者获取音量，最大值为1，0为静音
audioObject.loop = true

```
---
```
//设置或者获取循环状态
audioObject.duration //获取音乐长度
audioObject.currentTime //设置或者获取音乐当前播放的事件
audioObject.ended //判断音乐是否播放完毕，只读属性
```
### 事件
```
playing
当音乐开始播放，暂停后重新开始播放，设置currentTime后开始播放时触发
pause
当音乐暂停时和结束时触发
ended
当音乐结束时触发
timeupdate
当currentTime更新时会触发timeupdate，这个事件的触发频率由系统决定，但是会保证每秒触发4-66次（前提是每次事件处理不会超过250ms）
volumechange
当音量改变时触发
```
