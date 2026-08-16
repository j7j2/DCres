# DCres
Developing Countries low-res video encoding profile

# Introduction
This is not an application but a ffmpeg command / profile optimized for a certain use case

# Target devices
The video files encoded must be compliant with most of the old android 4.2 mobile phones and tablet

# Rules
Video will be 0.1mp and full mod16 (even if aspect ratio is slightly off)
there will be 3 aspect ratios:
2:1 to encode movies that are originally in 2.35:1
16:9
4:3
Audio will be downstreamed to mono. Fidelity before stereophony
Audio is either aac or mp3, mostly aac but mp3 for stuff like music shows so one can extract the track and copy it without re-encoding it to old legacy mp3 players
