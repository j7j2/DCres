# DCres
Developing Countries low-res multimedia encoding profiles

# What is DCres?
DCres is a fixed quality standard that adapts itself to the content  
0.1 MP (100,000px) at various aspect ratios & mod16 compliant  
Mono aac-he or mp3 audio  
subtitles in plain 3GPP timed text  

# Target devices
Compliant with most of the old android 4.2 mobile phones and tablet and up  
The new good enough "mobile quality" people are looking for when watching stuff on their mobile devices

# Target size
-Movies-  
300mb for 3per gb on sd cards  
230mb for 4per gb on sd cards or 3 on a cd-r  
-Tv Series- (45-50min)  
100mb per episode  
for short content such as videoclips or short movies, ...kbps average for the video track 

# Rules
-- VIDEO --  
Video is ~0.1mp and mod16, even if aspect ratio is slightly off, the "aspect" flag will take care of it  
there is 4 aspect ratios:  
2.264:1 480*208 if text on screen ended up getting cropped by 2:1  
2:1 to encode movies that are originally in 2.35-2.40 448*224  
16:9 432*240  
4:3  368*272  
Framerate will try to stick to the original source. 23.976/24/25/29.97/30 are allowed. For ntsc variants, do prefer fractional values for precision   
-- Audio --  
Audio will be downstreamed to mono. Fidelity before stereophony 
Some movies have hard to deal with voice track. A good example is Jupiter's Ascending. Good Luck making that movie sound intelligible on small speakers at their max volume  
Loud bursts will be compressed down with a fast attack and release using a multiband compressor so that the rumble of a train passing by does not bring down the overall volume of the scene  
Loudness will then be normalized so that action scenes and quiet ones end up to the same loudness  
Audio is either aac or mp3, mostly aac but mp3 for stuff like music shows so one can extract the track and copy it without re-encoding it to old legacy mp3 players  
AAC-HE-V1 is encoded at 48khz 35 kbps because those odd numbers are the upper limit before the encoder ramp up a notch the non-sdr audip bandwidth part giving it the most bit it can ( 27, 35, 43 do get better non-sdr quality than 28, 36 and 44)  
MP3 is encoded at 32khz v4 which averages to 64kbps and does sound better than its 44.1 or 48 khz counterpart at the same bitrate  

# Source material
The cleanest possible at the time of the encode  
Some dvd version of some movies are really sloppy, get the full blu-ray content  
avoid 4k content or be mindful that some of it is hdr and some isn't. hdr stuff need to have the proper tonemapping applied to them so they look good on sdr displays. that's a whole topic on its own  

# Editing
content will be edited to cut parts such as "previously in star trek enterprise", episodes in two parts or short movies in multiple parts that recap stuff at the beginning of the 2nd or 3rd part...
Generic at the end can be encoded with a monochrome filter and have their quality turned down compared to the rest of the movie  
