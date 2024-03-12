# AnotherRTSP

Tired of juggling between surveillance feeds and your daily tasks on your Windows system? Say goodbye to clunky interfaces and interruptions with AnotherRTSP.

AnotherRTSP is your ultimate solution for effortless monitoring of video cameras while maintaining peak productivity. Seamlessly integrating into your desktop environment, it ensures that surveillance never compromises your workflow. With its intuitive layout, you can arrange camera feeds in a single column, always within reach, without cluttering your workspace.

But here's the best part – AnotherRTSP isn't just another closed-door solution. It's a community-driven endeavor, open source and free for all to enhance. Designed with a focus on comfort and ergonomics, AnotherRTSP prioritizes your convenience above all else.

Experience the future of surveillance and productivity fusion with AnotherRTSP – where monitoring meets seamless work harmony!"


<img src="https://raw.githubusercontent.com/e1z0/AnotherRTSP/master/pictures/win11-with-mqttrules.jpeg" width="800" />

[More screenshots](../../wiki/Screenshots)

Introducing my latest software project: a cutting-edge RTSP stream player designed to revolutionize the way you interact with CCTV feeds. With intuitive controls and a host of advanced features, this application promises to enhance your surveillance experience like never before.
Streamlined Interface: Our RTSP stream player boasts a user-friendly interface that simplifies the process of monitoring multiple cameras simultaneously. Easily move video windows around your desktop and resize them to suit your preferences.
Customizable Layouts: Say goodbye to static setups. Our software remembers your preferred layout configurations, allowing you to effortlessly arrange and organize your camera feeds exactly how you want them.
Expandable Camera Support: Whether you're monitoring one camera or a dozen, our RTSP stream player accommodates your needs. Add as many cameras as necessary to keep tabs on various locations without limitations.
Keyboard Shortcut Integration: Take control with ease using keyboard arrow keys to resize video windows on-the-fly. This seamless integration enhances your efficiency, enabling quick adjustments without disrupting your workflow.

MQTT Integration: Harness the power of MQTT to set up customized alerts based on specific topics. Receive notifications directly within the application, keeping you informed of critical events in real-time.
Dynamic LED Lights: Visual cues are key to effective monitoring. Our software features built-in LED lights that dynamically respond to MQTT triggers, providing instant visual feedback for important events.
Sound Notifications: Stay informed even when you're not actively monitoring the feed. Receive audible alerts for critical events, ensuring you never miss a moment that requires your attention.
Future-Proof Features: Our commitment to innovation means that more features are on the horizon. Expect continuous updates and enhancements to further elevate your surveillance experience.

In summary, our RTSP stream player offers unparalleled convenience, flexibility, and functionality for CCTV monitoring. Experience the future of surveillance software today.

Description is generated by AI, lol, but as it says, it works pretty much as described.

# Real description

I've long searched for an alternative to the MacOS-exclusive RTSP player, SecuritySpy, I've never found anything like it. SecuritySpy has been incredibly convenient for me, seamlessly integrating into my desktop environment for monitoring video cameras while allowing me to carry out my daily tasks without any glitches. Its ability to arrange camera feeds neatly in a column, always accessible, is a feature any user would appreciate for its simplicity.

However, being tied to a Windows operating system, I haven't found anything comparable. Every program I've come across has been bulky and lacks the efficiency I'm accustomed to. Frustrated by the lack of options, I decided to take matters into my own hands and create my own solution.

Though initially modest in its capabilities, my homemade player fulfills its primary purpose – providing a seamless experience for monitoring cameras while working on the computer. Moreover, it's now freely available for anyone to use and improve, as it's open source.

This player doesn't aim to be a jack-of-all-trades; its focus is solely on providing comfort and ergonomics. No longer do cluttered camera windows hinder productivity – with this player, monitoring cameras and working concurrently is a breeze. Comfort and efficiency come first in this project, with additional features to follow suit.

I use such video surveillance tools as BlueIris and Frigate, so I didn't forget about them, as well as home automation, the program has integrated MQTT support, so it is possible to receive messages and react to them according to rules that you can create yourself. Whether it's a notification or another action, the app will let you integrate both movements and objects captured by the cameras. For example, if a person has entered the monitored area and the video surveillance system is set to recognize objects, you will receive a message directly on the desktop. Instead of messages it can be Sounds, Led Lights, Baloon tooltips and many more :)

# Technical abilities

Under the hood AnotherRTSP uses a library called LibEasyPlayer which is developed and maintained by TSINGSEE Qingxi Open Platform it is a Complete RTSP streaming media player project. LibEasyPlayer realizes real-time collection, decoding and display of RTSP live streams, which is stable, efficient and low-latency; decoding can use Intel hardware decoding and software decoding, and can perform real-time recording, snapshot capture, OSD overlay and other functions.
Video encoding supports H.264, H.265, MPEG4, MJPEG, and audio supports G711A, G711U, G726, AAC. Supports RTSP over TCP/UDP protocol, supports soft/hard decoding, and is an excellent set of playback components for security streaming media platforms! LibEasyPlayer has gone through many years of development and iteration, and has been used in many commercial projects. It has become very stable and complete. Its functions include: live broadcast, video recording, and screenshots. It should be said that it has the most functionality, stability and completeness on the market. A powerful RTSP player library!

Most domestic RTSP/RTP protocol players are based on ffmpeg (including the protocol layer and decoding layer). However, in the actual implementation of RTSP/RTP projects, due to the differences in the custom fields of each manufacturer, many Special compatibility is required, which is what ffmpeg players cannot achieve. LibEasyPlayer relies on the huge EasyDarwin user group and has adapted it to almost all domestic camera manufacturers. It is very compatible and very stable!

Currently supported features list:

- [x] Ultra-low latency RTSP player;
- [x] Super device compatibility and customizability;
- [x] Perfectly supports multi-window and multi-instance playback;
- [ ] Support RTSP TCP/UDP mode switching;
- [ ] Supports real-time setting of the playback buffer and mature low-latency frame tracking technology;
- [x] Turn on the playback function in seconds;
- [x] Support custom playback layout;
- [x] The codec, display, and playback source codes are fully open, making it more flexible;
- [ ] Support OSD text watermark;
- [x] Support real-time recording and instant picture taking;
- [ ] Detailed log output callback;

# Usage

[See usage information on wiki](../../wiki/Usage)

# Roadmap

[See wiki page](../../wiki/Roadmap)

# Operating System support

* Windows XP (see the [wiki topic](../../wiki/Windows-XP-Support))
* Windows Vista
* Windows 7
* Windows 8
* Windows 8.1
* Windows 10
* Windows 11

# Third party Components used

* EasyPlayerRTSP Libraries https://github.com/tsingsee/EasyPlayer-RTSP-Win
* Paho MQTT m2mqtt 4.3.0.0 (2017.05.20)
* Tiny-JSON v1.2.0 https://github.com/gering/Tiny-JSON
