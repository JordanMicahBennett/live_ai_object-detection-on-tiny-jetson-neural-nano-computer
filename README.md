This is successful execution of the ubuntu mini-neural computer jetson nano hardware running ai based object detection, using 
the [jetson nano detection and tracking kit](https://github.com/SteveMacenski/jetson_nano_detection_and_tracking).

This kit is a small neural-computer with 128 tegra cores, which runs machine learning tools and libraries designed for arm usage. 
As the small neural computer comes without ability to boot, one is first required to prepare a disk image on a micro sd card using something other than the aforesaid jetson-nano neural computer, and I used my desktop to perform the tasks below.



Steps I took:

1. Via [budgetpcja](https://www.facebook.com/budgetpcja/), I bought and shipped [jetson-nano-kit](https://www.amazon.com/Jetson-Nano-Developer-Kit-Package/dp/B07RQRMXQ6), 253 usd. (Took a week to arrive here to Jamaica)

2. For the purpose of running nano sdk/OS on nano, using an i7 Desktop (that I also bought and shipped through [budgetpcja](https://www.facebook.com/budgetpcja/), I flashed a 64 gig micro sd card that comes with kit above, according to [a relevant nvidia guide](https://developer.nvidia.com/embedded/learn/get-started-jetson-nano-devkit) Took about half an hour or less.

3. Finally, booted small jetson nano neural computer on the flashed micro sd card, before which I had assembled kit, plus used usb keyboard, wifi adaptor, usb mouse. (Took maybe ~30 minutes to get booted result, where I could login to the nano)

4. Taking about 5 hours (slow internet connection at home) I then installed the [jetson nano detection and tracking kit](https://github.com/SteveMacenski/jetson_nano_detection_and_tracking). This kit allows us to run an ai based (convolutional neural network etc) object detection model. 

5. Oops, one reason why [the kit](https://github.com/SteveMacenski/jetson_nano_detection_and_tracking) failed to work at first, but then I suspected I didn't install the camera properly. The camera must be placed on the board in a particular order, which I discovered [here](https://medium.com/@dmccreary/getting-your-camera-working-on-the-nvida-nano-336b9ecfed3a).

6. Another reaosn why the kit failed to work first, was due to a "canberry error". A quick "sudo-apt get install libcanberra-gtk-module" fixed that error.

7. After doing the above, [the ai kit](https://github.com/SteveMacenski/jetson_nano_detection_and_tracking) with the ability to detect objects in camera stream, as I captured in the clip below:
