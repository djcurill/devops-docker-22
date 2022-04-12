# Exercise
Image devopsdockeruh/simple-web-service creates a timestamp every two seconds to /usr/src/app/text.log when it's not given a command. Start the container with bind mount so that the logs are created into your filesystem.

Submit the command you used to complete the exercise.

# Solution
sudo docker run --rm -it -v $(pwd):/usr/src/app/text.log -w /usr/src/app/text.log devopsdockeruh/simple-web-service