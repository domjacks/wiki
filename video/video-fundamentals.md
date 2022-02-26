# Video Fundamentals

## Scanning methods

Interlaced vs. Progressive

## Frame Rate

50Hz vs 60Hz

## Bitrates

### Variable bitrate

As opposed to CBR (constant bitrate), variable bitrate allows the amount of data per segment to be different. Meaning we can have a higher bitrate in more complex segments.

This is great for things like storage considerations where you want high bitrates (meaning high storage) for parts of the video but want to save space for less complex parts.  

### Adaptive bitrate

This is a strategy commonly used in video streaming to change the bitrate of the content based on conditions of the device such as network capacity.

## Aspect Ratios

- 16:9
- 

## Resolutions

### SD

- 720 x 480

### HD & FHD

- 1280 x 720
- 1920 x 1080

### UHD

- 3840 x 2160 (4K)
- 7680 x 4320 (8K)

> Technically 4K was first coined as a cinema standard of 4096x2160, but the 4K referred to in TV terms is 3840x2160.

## Colours and Contrast

Where increasing the number of pixels is a common way to try and increase quality, improving the pixels themselves can often lead to better perceived quality. 

### Dynamic Range

Dynamic range in video essentially means the range of contrast available for each pixel. Essentially, how much light each pixel should put out. This is called luminance.
 
#### High Dynamic Range

Previously, video signals had a limited range of contrast available to them.

HDR allows for darker blacks and lighter whites causing more depth to images.

There are many competing standards for HDR: HDR10, Dolby Vision, HLG

##### HLG

Hybrid Log Gamma is a standard developed by the BBC and NHK. It is notable as it provides a format that broadcasters could use, as well as being backwards-compatible for SDR.

It doesn't use any metadata at all and instead uses both the logarithmic and gamma curves used by TVs to calculate brightness for SDR and HDR. 

HLG can be referring to the transfer function or the format.

##### PQ

PQ is an alternative transfer function to HLG that is used as basis of a range of HDR formats such as Dolby Vision, HDR10 and PQ10.
###### Dolby Vision

Propriety format from Dolby. It utilises dynamic metadata, meaning it can adjust the luminance for each scene (or even frame).

Both a device and content has to be certified in order to be classified as Dolby Vision capable. Dolby works with TV manufacturers and content providers to also set some static metadata to tailor the experience.

###### HDR10 

HDR10 is an open standard that uses static metadata to ensure it is consistent across all devices. 

###### HDR10+

Samsung have developed their own format which builds upon HDR10 but adds some dynamic metadata. It is still an open standard. 

###### PQ10

System developed by Dolby that can be used on both images and video. It is essentially the same as HDR10 but without the metadata.

### Colour Gamut

Colour gamut is the range of colours available for each pixel. This is called chromacity.

#### WCG 

Wide Color Gamut.

Increases range of colors than the standard.

Allows for "redder" reds and "greener" greens.

> Often found with HDR, but it is not necesarily linked.

### Specifications

The two main specifications are BT.709 and BT.2020.

Both these specs contain information regarding the dynamic range and colour gamut that should be available. 

> DCI-P3 is another spec which is used for cinema
