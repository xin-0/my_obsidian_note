reference: 
https://fzheng.me/2016/01/08/ffmpeg/
https://trac.ffmpeg.org/wiki/How%20to%20speed%20up%20/%20slow%20down%20a%20video
adjust playback speed:
```
ffmpeg -i TheOrigin.mp4 -vf  "setpts=0.5*PTS" UpTheOrigin.mp4
```
frame rate the same as previous, playback speed x2

