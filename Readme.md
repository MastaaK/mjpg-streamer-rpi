[![Codefresh build status]( https://g.codefresh.io/api/badges/build?repoOwner=MastaaK&repoName=mjpg-streamer-rpi&branch=master&pipelineName=mjpg-streamer-rpi&accountName=mastaak&type=cf-2)]( https://g.codefresh.io/repositories/MastaaK/mjpg-streamer-rpi/builds?filter=trigger:build;branch:master;service:5a57b90b9579e10001d2d3d2~mjpg-streamer-rpi)

# ARM container for Mjpg-Streamer

## Genesis
This is my attempt to make the lightest container for ARM devices being buildable from any plateform and containing the bar minimum to make Mjpg-Streamer work. 

It's main purpose is to stream to [OctoPrint](https://octoprint.org/) and [Home Assistant](https://home-assistant.io/)

Compiled plugins: input_testpicture.so, output_autofocus.so, output_http.so, input_uvc.so, output_file.so

## To make it work

docker run -d -p hostport:80 --device=/dev/video0 --name=Mjpg-Streamer mastaak/mjpgstreamerrpi:master
