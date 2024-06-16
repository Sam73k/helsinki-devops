The Secret message is: 
    'You can find the source code here: https://github.com/docker-hy'

Commands
$ docker run -d --rm -it --name looper devopsdockeruh/simple-web-service:ubuntu                                           
Unable to find image 'devopsdockeruh/simple-web-service:ubuntu' locally
ubuntu: Pulling from devopsdockeruh/simple-web-service
5d3b2c2d21bb: Pull complete 
3fc2062ea667: Pull complete 
75adf526d75b: Pull complete 
965d4bbb586a: Pull complete 
4f4fb700ef54: Pull complete 
Digest: sha256:d44e1dce398732e18c7c2bad9416a072f719af33498302b02929d4c112e88d2a
Status: Downloaded newer image for devopsdockeruh/simple-web-service:ubuntu
WARNING: The requested image's platform (linux/amd64) does not match the detected host platform (linux/arm64/v8) and no specific platform was requested
d0fae1686f1a658a0b87f35745b8b48e512896aa3a35fb1a79c8d2ebe0ed5c9a
$ docker ps -a
CONTAINER ID   IMAGE                                      COMMAND                  CREATED          STATUS          PORTS     NAMES
d0fae1686f1a   devopsdockeruh/simple-web-service:ubuntu   "/usr/src/app/server"    28 seconds ago   Up 28 seconds             looper
root@d0fae1686f1a:/usr/src/app# tail -f ./text.log
Secret message is: 'You can find the source code here: https://github.com/docker-hy'
2024-06-16 11:03:43 +0000 UTC
2024-06-16 11:03:45 +0000 UTC
2024-06-16 11:03:47 +0000 UTC
2024-06-16 11:03:49 +0000 UTC
2024-06-16 11:03:51 +0000 UTC
Secret message is: 'You can find the source code here: https://github.com/docker-hy'
2024-06-16 11:03:53 +0000 UTC
2024-06-16 11:03:55 +0000 UTC
2024-06-16 11:03:57 +0000 UTC
2024-06-16 11:03:59 +0000 UTC
2024-06-16 11:04:01 +0000 UTC
Secret message is: 'You can find the source code here: https://github.com/docker-hy'
2024-06-16 11:04:03 +0000 UTC
2024-06-16 11:04:05 +0000 UTC
2024-06-16 11:04:07 +0000 UTC
2024-06-16 11:04:09 +0000 UTC
2024-06-16 11:04:11 +0000 UTC
Secret message is: 'You can find the source code here: https://github.com/docker-hy'