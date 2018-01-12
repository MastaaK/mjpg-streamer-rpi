[![Codefresh build status]( https://g.codefresh.io/api/badges/build?repoOwner=MastaaK&repoName=mjpg-streamer-rpi&branch=master&pipelineName=mjpg-streamer-rpi&accountName=mastaak&type=cf-2)]( https://g.codefresh.io/repositories/MastaaK/mjpg-streamer-rpi/builds?filter=trigger:build;branch:master;service:5a57b90b9579e10001d2d3d2~mjpg-streamer-rpi)
mjpg-streamer Dockerfile

Mjpg-Streamer for RPi. Mainly created to work w/ Octoprint and Home-Assistant

Compiled plugins: input_testpicture.so, output_autofocus.so, output_http.so, input_uvc.so, output_file.so

docker run -d -p 80 --device=/dev/video0 --name=Mjpg-Streamer mastaak/mjpgstreamerrpi:master
