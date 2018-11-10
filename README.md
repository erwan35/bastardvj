Bastardvj tends to be be a simple all-in-one veejaying patch for 
Pure Data.

It was originaly created in 2007 but I wanted to see if this was still 
working after more than 10 years. It might also provide people with some 
ideas.

It was quite stable and used during live sessions without problems and
was working smoothly on a celeron 1.4ghz.

![Screenshot](/doc/screenshot.png)

# What's needed :
- Ubuntu 18.04 (but might work elsewhere for sure)
- Pure Data (tested on 0.48.1), pd-pdp and pd-unauthorized from the ubuntu repo
- pidip from https://github.com/caedesvvv/pidip-caedes
  I'm able to compile the "official" pidip from http://ydegoyon.free.fr/pidip.html
  but it's not being loaded by PureData

# Usage
- run ./bastard.vj.sh
- configure the path to your videos and images in pd conf (a box in
  the bottom left of the patch).
- Choose a video in the left playlist-abs (it should trigger a pdp 
  video window) and then a video in the right playlist-abs. Use the 
  central big mixer to mix the 2 videos.
- The speed and "randomness" can also be controlled.
- With Blanco and Negro buttons, black or white videos are sent to
  "clean" the pdp window (these 2 videos files are included into the
  distributions).
- Effects : try yourself :)
- Webcam : open it (v4l) and mix it
- Images : can be "blended by the sound"
- DSP : Music can be routed to the patch (through Jackd for example).
  The purple toggles will be triggered by some messages coming from the bonk 
  object (very simple sound computation).

# Troubleshooting
- if the pdp window is not appearing try to change pdp_glx to pdp_xv 
  (it means that your opengl stuff is not working correctly or that
  you don't have an opengl on your system).
- be sure that pdp, pidip, countund, playlist are loaded

Greetings to Acracia, Rama, Lluis, Caedes, Mose and the Pure Data community !
