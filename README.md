This is successful execution of the ubuntu mini-neural computer jetson nano hardware running ai based object detection, using 
the [jetson nano detection and tracking kit](https://github.com/SteveMacenski/jetson_nano_detection_and_tracking).

This kit is a small neural-computer with 128 tegra cores, which runs machine learning tools and libraries designed for arm usage. 
As the small neural computer comes without ability to boot, one is first required to prepare a disk image on a micro sd card using something other than the aforesaid jetson-nano neural computer, and I used my desktop to perform the tasks below.



Steps I took:

1. I bought and shipped through [budgetpcja](https://www.facebook.com/budgetpcja/), [jetson-nano-kit](https://www.amazon.com/Jetson-Nano-Developer-Kit-Package/dp/B07RQRMXQ6), 253 usd. (Took a week to arrive here to Jamaica)

2. For the purpose of running nano sdk/OS on nano, using an i7 Desktop (that I also bought and shipped through [budgetpcja](https://www.facebook.com/budgetpcja/), I flashed a 64 gig sd card that comes with kit above, according to [a relevant nvidia guide](https://developer.nvidia.com/embedded/learn/get-started-jetson-nano-devkit) Took about half an hour or less.

3. Finally, booted small jetson nano neural computer, before which I had assembled kit, plus used usb keyboard, wifi adaptor, usb mouse. (Took maybe ~30 minutes to get booted result, where I could login to the nano)

4. Taking about 5 hours (slow internet connection at home) I then installed the [jetson nano detection and tracking kit](https://github.com/SteveMacenski/jetson_nano_detection_and_tracking). This kit allows us to run an ai based (convolutional neural network etc) object detection model. 
