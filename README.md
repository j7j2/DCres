# DCres
Developing Countries low-res video encoding profile

# Introduction
This is not an application but a ffqueue profile set optimized for a certain use case

# Target devices
The video files encoded must be compliant with most of the old android 4.2 mobile phones and tablet

# Target size
300mb for 3per gb on sd cards
230mb for 4per gb on sd cards or 3 on a cd-r

# Rules
Video will be 0.1mp and full mod16 (even if aspect ratio is slightly off)  
there will be 3 aspect ratios:  
2:1 to encode movies that are originally in 2.35:1  448*224  
16:9 432*240  
4:3  368*272  
Framerate will try to stick to the original source. 23.976/24/25/29.97/30 are allowed.  
Audio will be downstreamed to mono. Fidelity before stereophony  
Audio is either aac or mp3, mostly aac but mp3 for stuff like music shows so one can extract the track and copy it without re-encoding it to old legacy mp3 players

# Editing
content will be edited to cut parts such as "previously in star trek enterprise", episodes in two parts or short movies in multiple parts that recap stuff at the beginning of the 2nd or 3rd part...
