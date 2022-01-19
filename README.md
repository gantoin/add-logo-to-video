# Add your logo on video !
How to easily tag a video with your logo via a simple ffmpeg command

```bash
ffmpeg -i video.mp4 -i logo.png -filter_complex "[1]format=rgba,colorchannelmixer=aa=0.5[logo];[0][logo]overlay=5:5:format=auto,format=yuv420p" -c:a copy tag-video.mp4
```

# Before
![before](video.gif)


# After!
[after](video_tag.gif)

