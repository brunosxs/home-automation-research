# DVR

Cameras and any device that will integrate the DVR pipeline should be powered through [POE](https://en.wikipedia.org/wiki/Power_over_Ethernet).
This facilitates the instalation immensily and is less of a hindrance as you only have a single cable to connect from the server to the camera. This is inegotiable.

## Questions:

### Should I go for a pre-built DVR and just use a NAS to periodically backup videos?
Maybe, but this would limit integration between my network and the cctv system. But I am open to the possibility to simply buy a prebuilt one. In this case, it NEEDS to have a proper and good way to do unnatended backups and look into the camera feed. For backups, if I have rsync or ssh that should be more than enough, but I am not sure about accessing the video feeds from the DVR.

### Will my NAS be able to handle the cameras plus its usual work?
I am pretty certain it won´t. So I should probably reserve one mini-pc for this all while I add cronjobs to backup and do other stuff to the NAS.

## Hardware

- At least support for 8 cameras
- Cameras should have night-vision and at least 720p resolution (1080 prefered)
- x264, x265 or av1 encoding (no proprietary bullshit)
- POE switch that should have 2.5gbps uplink to the actual server. 


## Software to look into:

### [Frigate](https://docs.frigate.video/)

Initial impression is promissing.Seems to accept any camera that uses ip protocol to send data.