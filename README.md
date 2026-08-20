# DCres
Developing Countries low-res multimedia encoding profiles

# What is DCres?
DCres is a fixed quality standard that adapts itself to the content  
0.1 MP (100,000px) at various aspect ratios & mod16 compliant  
Mono aac-he or mp3 audio  
subtitles in plain 3GPP timed text  

# Target devices
Compliant with most of the old android 4.2 mobile phones and tablet and up

# Target size
-Movies-  
300mb for 3per gb on sd cards  
230mb for 4per gb on sd cards or 3 on a cd-r  
-Tv Series- (45-50min)  
100mb per episode  
for short content such as videoclips or short movies, 200kbps average for the video track  

# Rules
Video will be 0.1mp and full mod16 (even if aspect ratio is slightly off)  
there is 4 aspect ratios:  
2.4 from 1920*800
2:1 to encode movies that are originally in 2.35-2.40  448*224  
16:9 432*240  
4:3  368*272  
Framerate will try to stick to the original source. 23.976/24/25/29.97/30 are allowed.  
Audio will be downstreamed to mono. Fidelity before stereophony  
Audio is either aac or mp3, mostly aac but mp3 for stuff like music shows so one can extract the track and copy it without re-encoding it to old legacy mp3 players

# Editing
content will be edited to cut parts such as "previously in star trek enterprise", episodes in two parts or short movies in multiple parts that recap stuff at the beginning of the 2nd or 3rd part...
