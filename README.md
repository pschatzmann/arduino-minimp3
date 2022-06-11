# arduino-minimp3

Minimalistic, single-header library for decoding MP3. minimp3 is designed to be small, fast (with SSE and NEON support), and accurate (ISO conformant). Further information can be found in the [oringal readme](README.original).

I have extended the project, so that it can be used as Arduino library. The result however is not very convincing: The decoder is too slow (e.g. on an ESP32) to decode any audio with a rate >= 32000 samples per second and the audio quality is quite poor. 


### Installation in Arduino

You can download the library as zip and call include Library -> zip library. Or you can git clone this project into the Arduino libraries folder e.g. with

```
cd  ~/Documents/Arduino/libraries
git clone pschatzmann/arduino-minimp3.git
```

I recommend to use git because you can easily update to the latest version just by executing the ```git pull``` command in the project folder.

### Documentation

I recommend to use this library together with my [Arduino Audio Tools](https://github.com/pschatzmann/arduino-audio-tools). 
This is just one of many __codecs__ that I have collected so far: Further details can be found in the [Encoding and Decoding Wiki](https://github.com/pschatzmann/arduino-audio-tools/wiki/Encoding-and-Decoding-of-Audio) of the Audio Tools.

