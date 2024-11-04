# csi_camera

# Linux command
$ git clone 
$
$

# Windows command
open powershell
>gst-launch-1.0 -v udpsrc port=8001 ! ‘application/x-rtp,encoding-name=(string)H264,payload=(int)96’ ! rtph264depay ! queue ! avdec_h264 ! videoconvert! autovideosink ![image](https://github.com/user-attachments/assets/688f8533-f8e3-453a-b902-2037d1cd2d80)

open new powershell
>gst-launch-1.0 -v udpsrc port=8002 ! ‘application/x-rtp,encoding-name=(string)H264,payload=(int)96’ ! rtph264depay ! queue ! avdec_h264 ! videoconvert! autovideosink ![image](https://github.com/user-attachments/assets/7a5f0f85-7e1b-4e69-a08f-3f1becc14f48)
