# CrowdWatcher

This project is the open-source eye tracking platform `CrowdWatcher`. It enables researchers to measure visual attention and user engagement in a crowdsourcing context through traditional RGB webcams. 

Its general idea is to use conventional RGB cameras, such as the one provided with a laptop, to measure where the participants are looking on the screen faced to them. The key aspect of the platform is to use the interactions of the user with his computer as a way to perform an online calibration of the eye tracker. Indeed, it is expected that when a participant performs an action such as a click, he will be looking at the position on the screen while performing the click. Therefore, at the very moment of the click, it is possible to relate pupil center position from the video stream to a position on the screen. Based on this principle, a browser-based real- time audio/video processing using WebRTC was developed enabling to perform tests in a crowdsourcing context.

The platform has two parts: a client and a server side. The client side employs WebRTC to turn on the camera of the participants and record their face while performing the task, and in parallel record actions of the user with the platform. 

The server side of the platform is in charge of delivering the content to the client, retrieving the measurements performed on the client side, and performing the fixations estimations based on the webcam video stream and user actions logs.


# Access

The project is hosted on the GitHub account of the group Audio Visual Technology of TU Ilmenau (Germany). 
https://github.com/Telecommunication-Telemedia-Assessment/CrowdWatcher