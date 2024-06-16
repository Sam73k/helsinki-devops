$ docker run -d nginx      
Unable to find image 'nginx:latest' locally
latest: Pulling from library/nginx
559a76444520: Pull complete 
6d49e2cc7379: Pull complete 
de7de5956f3a: Pull complete 
d3756208472d: Pull complete 
8e17037a07ce: Pull complete 
1879d5982048: Pull complete 
c06f6b42c3b9: Pull complete 
Digest: sha256:56b388b0d79c738f4cf51bbaf184a14fab19337f4819ceb2cae7d94100262de8
Status: Downloaded newer image for nginx:latest
6f4a2bafd783427dc9cd074accbf7aa679ea600494e290e28ea22d21ae86dc0e
$ docker run -d nginx
7768a833b29fccc158753c97c04ed0fedebbb94f9f63bb143f537e2202f7b8eb
$ docker run -d nginx
148f7e2de3c66cf901cbb10647bb0f295e81e7fe8c55fa49179316384a57cd90
$ docker ps -a
CONTAINER ID   IMAGE     COMMAND                  CREATED              STATUS              PORTS     NAMES
148f7e2de3c6   nginx     "/docker-entrypoint.…"   5 seconds ago        Up 4 seconds        80/tcp    sweet_edison
7768a833b29f   nginx     "/docker-entrypoint.…"   6 seconds ago        Up 6 seconds        80/tcp    dreamy_shtern
6f4a2bafd783   nginx     "/docker-entrypoint.…"   About a minute ago   Up About a minute   80/tcp    crazy_darwin
$ docker stop sweet_edison dreamy_shtern
sweet_edison
dreamy_shtern
$ docker ps -a                          
CONTAINER ID   IMAGE     COMMAND                  CREATED          STATUS                     PORTS     NAMES
148f7e2de3c6   nginx     "/docker-entrypoint.…"   51 seconds ago   Exited (0) 7 seconds ago             sweet_edison
7768a833b29f   nginx     "/docker-entrypoint.…"   52 seconds ago   Exited (0) 7 seconds ago             dreamy_shtern
6f4a2bafd783   nginx     "/docker-entrypoint.…"   2 minutes ago    Up 2 minutes               80/tcp    crazy_darwin