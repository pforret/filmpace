# Scene detect with ffmpeg

Can we detect montage speed of a video? Where 0 = static image, and 1 = 1 scene change per second (very frantic)

- https://jdhao.github.io/2021/12/25/ffmpeg-extract-key-frame-video/

ffmpeg -i input.mp4 -vf "select='gt(scene,0.4)'" -vsync vfr frame-%2d.jpg



