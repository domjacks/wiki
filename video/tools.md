# Tools

## FFMPEG

Convert .mov to .mp4:
`ffmpeg -i my-video.mov -vcodec h264 -acodec aac my-video.mp4`

Copy video without audio:
`ffmpeg -i chameleon.mp4 -c:v copy -an videoWithoutAudio.mp4`

## MP4Box

Create DASH stream from MP4:
`mp4box -dash 3840ms -segment-name segment_ my-video.mp4`