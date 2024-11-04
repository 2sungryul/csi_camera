# csi_camera

# Linux command

$ git clone https://github.com/2sungryul/csi_camera.git

$ cd csi_camera

$ make 

$ ./camera

# Windows command

open powershell

PS> gst-launch-1.0 -v udpsrc port=8001 ! ‘application/x-rtp,encoding-name=(string)H264,payload=(int)96’ ! rtph264depay ! queue ! avdec_h264 ! videoconvert! autovideosink

open new powershell

PS> gst-launch-1.0 -v udpsrc port=8002 ! ‘application/x-rtp,encoding-name=(string)H264,payload=(int)96’ ! rtph264depay ! queue ! avdec_h264 ! videoconvert! autovideosink
