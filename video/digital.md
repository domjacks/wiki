# Digital Video

## Formats

Standard set of rules for storing containers, codecs, metadata and folder structure.

### MP4

The term "MP4" can be used to refer to the format, container, H.264 codec, ISO Base Media File so it can be quite confusing.

> Note: See [Streaming](./streaming.md) for information on formats used for streaming

## Container

Containers _contain_ all the information regarding the video or audio file. They contain the video and audio streams, as well as any meta data.

The metadata contains information about things like:

* Bitrate
* Resolution
* Codec
* Subtitles
* Timestamps
* ...

### MP4

### WebM

### IVF

## Codecs

**Co**der + **Dec**oder.

Lots and lots of both proprietary and open source codecs for audio and video.

### Video Codecs

#### H.264 / AVC

* Most common video codec

#### H.265 / HEVC

* Proprietary
* Successor to H.264
* Half the bitrate of H.264
* Good for high resolutions and live streaming
* A lot more resources needed to encode
* Not as widely supported

#### VP9

* Royalty-free and open source codec
* Half the bitrate of VP8
* Good for high resolutions and live streaming
* A lot more resources needed to encode
* Not as widely supported

#### AV1

* Royalty-free and open source codec

### Audio Codecs

#### MP3

* Widely supported
* Saves space without noticeable quality loss
* Limited functionality

#### AAC (Advanced Audio Coding)

* Widely supported
* More efficient than MP3 (better sound for same bitrate)
* Limit on audio channels

#### AC-3 (Dolby Digital Audio Codec 3)

* More audio channels (5.1)
* Not as widely supported
