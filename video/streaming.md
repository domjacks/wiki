# Streaming

Streaming video is all about IP-delivered video being streamed to a user's device continuously.

## Streaming Protocols

Streaming protocols are digital formats for video and audio content. They are tailored for online streaming by splitting the content into multiple smaller segments and describing this content via metadata. Players know how to interpret these formats and thus stream the content.

### DASH

MPEG Dynamic Adaptive Streaming over HTTP.

MPEG DASH is an open source standard for streaming content. It uses an XML manifest file to describe content.

* `.mpd` - Manifest file
* `.m4s` - Media Segment

### HLS

HTTP Live Streaming. Proprietary format created by Apple.

* `.m3u8` - Playlist file
* `.ts` - Media Segment

## Progressive Download

Progressive Download is a type of pseudo-streaming. Where it differs from the standard streaming protocols is it does not support ABR.

A simple example of progressive download in the web world would be to have a simple `<video>` element with a `src` attribute pointing to an `mp4` file:

```
<video src="my-video.mp4"></video>
```

In this case, the browser knows to continually buffer the video and allow the player to play as soon as a decent enough amount of content is buffered.

## Low Latency Streaming