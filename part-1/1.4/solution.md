$ docker run -d -it ubuntu sh -c 'while true; do echo "Input website:"; read website; echo "Searching.."; sleep 1; curl http://$website; done'
$ docker image ls
REPOSITORY   TAG       IMAGE ID       CREATED       SIZE
ubuntu       latest    28bc33afd4c9   2 weeks ago   98.8MB
$ docker ps -a
CONTAINER ID   IMAGE     COMMAND                  CREATED          STATUS          PORTS     NAMES
2d5e1918f38b   ubuntu    "sh -c 'while true; …"   14 seconds ago   Up 13 seconds             elastic_brahmagupta
$ docker exec -it elastic_brahmagupta bash
    # apt-get update
    # apt-get install -y curl
    # exit

$ docker attach elastic_brahmagupta
helsinki.fi
Searching..
<html>
<head><title>301 Moved Permanently</title></head>
<body>
<center><h1>301 Moved Permanently</h1></center>
<hr><center>nginx/1.22.1</center>
</body>
</html>