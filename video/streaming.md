# Streaming

Streaming video is all about IP-delivered video being delivered to a user's device continuously

## Streaming Protocols

### DASH

MPEG Dynamic Adaptive Streaming over HTTP

### HLS

HTTP Live Streaming

## Progressive Download

Progressive Download is a type of pseudo-streaming. Where it differs from the standard streaming protocols is it does not support ABR.

A simple example of progressinve download in the web world would be to have a simple `<video>` element with a `src` attribute pointing to an `mp4` file:

```
<video src="my-video.mp4"></video>
```

## Low Latency Streaming