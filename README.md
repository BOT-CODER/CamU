# CamU v1.1
Take webcam shots from target just sending a malicious link

![Cam You](https://i.ibb.co/yY0WZtM/IMG-20191024-223723.jpg)
# How it works?
<p>The tool generates a malicious HTTPS page using Serveo or Ngrok Port Forwarding methods, and a javascript code to cam requests using MediaDevices.getUserMedia. </p>

<p>The MediaDevices.getUserMedia() method prompts the user for permission to use a media input which produces a MediaStream with tracks containing the requested types of media. That stream can include, for example, a video track (produced by either a hardware or virtual video source such as a camera, video recording device, screen sharing service, and so forth), an audio track (similarly, produced by a physical or virtual audio source like a microphone, A/D converter, or the like), and possibly other track types. </p>

[See more about MediaDEvices.getUserMedia() here](https://developer.mozilla.org/en-US/docs/Web/API/MediaDevices/getUserMedia)
<p> To convince the target to grant permissions to access the cam, the page uses a javascript code made by https://github.com/wybiral that turns the favicon into a cam stream.</p>

## Installing (Kali Linux/Termux):

```
apt update -y
apt install git
git clone https://github.com/BOT-CODER/CamU.git
cd CamU
bash setup.sh
python CamU.py
```

## One line Installation:

```
apt update && apt install git && git clone https://github.com/BOT-CODER/CamU.git && cd CamU && bash setup.sh && python CamU.py
```