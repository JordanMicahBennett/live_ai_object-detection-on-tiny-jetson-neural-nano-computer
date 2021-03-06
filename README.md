This is successful execution of the ubuntu mini-neural computer jetson nano hardware running ai based object detection, using 
the python [jetson nano software detection and tracking kit](https://github.com/SteveMacenski/jetson_nano_detection_and_tracking).

The [jetson hardware kit](https://www.amazon.com/Jetson-Nano-Developer-Kit-Package/dp/B07RQRMXQ6) is a small neural-computer with 128 tegra cores, which runs machine learning tools and libraries designed for arm usage. 

As the small neural computer comes without ability to boot, one is first required to prepare a disk image on a micro sd card using something other than the aforesaid jetson-nano neural computer, and I used my desktop to perform said disk preperartion task.



Steps I took:
===
1. Via [budgetpcja](https://www.facebook.com/budgetpcja/), I bought and shipped [jetson-nano-kit](https://www.amazon.com/Jetson-Nano-Developer-Kit-Package/dp/B07RQRMXQ6), for 253 USD, which comes with a tiny lcd screen seen in success video below, adaptor, appropriate usb and hdmi cords, small Rpi camera. I also separately bought a case to cover the nano-board, and a reflective film. (Took a week for kit to arrive here to Jamaica)

2. For the purpose of running nano sdk/OS on nano, using an i7 Desktop (that I also bought and shipped through [budgetpcja](https://www.facebook.com/budgetpcja/)), I flashed a 64 gig micro sd card that comes with kit above, according to [a relevant nvidia guide](https://developer.nvidia.com/embedded/learn/get-started-jetson-nano-devkit) Took about half an hour or less.

3. Finally, booted small jetson nano neural computer on the flashed micro sd card, before which I had assembled kit, plus used usb keyboard, wifi adaptor, usb mouse. (Took maybe ~30 minutes to get booted result, where I could login to the nano)

4. Taking about 5 hours (slow internet connection at home) I then installed the [jetson nano detection and tracking kit](https://github.com/SteveMacenski/jetson_nano_detection_and_tracking). This kit allows us to run an ai based (convolutional neural network etc) object detection model. 

5. Oops, one reason why [the kit](https://github.com/SteveMacenski/jetson_nano_detection_and_tracking) failed to work at first, is as I suspected; I didn't install the camera properly. The camera must be placed on the board in a particular order, which I discovered [here](https://medium.com/@dmccreary/getting-your-camera-working-on-the-nvida-nano-336b9ecfed3a).

6. Another reason why the kit failed to work first, was due to a "canberra error". A quick "sudo-apt get install libcanberra-gtk-module" fixed that error.

Success! 
===
After doing the above, [the ai kit](https://github.com/SteveMacenski/jetson_nano_detection_and_tracking) can now detect objects in camera stream right on the jetson nano mini neural computer, without need to connect to my somewhat powerful i7 desktop (as I captured in the clip below): 

[Youtube/Live Ai object detection on tiny jetson nano neural computer](https://www.youtube.com/watch?v=Vp93UgLiq-w&feature=youtu.be)

At minute [1:00](https://www.youtube.com/watch?v=Vp93UgLiq-w&t=60s) from video above, the ai model detects my work id which is cool.



Future plans
===
I also bought a reflective film along with the kit, which is to be placed on my car's windshield, to reflect the small lcd screen that came with nano kit. Now working on a project to help warn driver of road conditions. The warnings will be visible to the driver via the reflective film. See [this video](https://www.youtube.com/watch?v=cfUmRj976qE) which shows a speedometer on reflective film/hud. I will do something like the video, but with ai based road condition warnings instead of speedometer numbers.
