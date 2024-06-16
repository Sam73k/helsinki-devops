$ docker ps -a                          
CONTAINER ID   IMAGE     COMMAND                  CREATED          STATUS                     PORTS     NAMES
148f7e2de3c6   nginx     "/docker-entrypoint.…"   51 seconds ago   Exited (0) 7 seconds ago             sweet_edison
7768a833b29f   nginx     "/docker-entrypoint.…"   52 seconds ago   Exited (0) 7 seconds ago             dreamy_shtern
6f4a2bafd783   nginx     "/docker-entrypoint.…"   2 minutes ago    Up 2 minutes               80/tcp    crazy_darwin
$ docker image ls
REPOSITORY   TAG       IMAGE ID       CREATED       SIZE
nginx        latest    11ceee7cdc57   2 weeks ago   193MB
$ docker stop 14 77 6f
14
77
6f
$ docker rm 14 77 6f
14
77
6f
$ docker ps -a
CONTAINER ID   IMAGE     COMMAND   CREATED   STATUS    PORTS     NAMES
$ docker image rm -f 11
Untagged: nginx:latest
Untagged: nginx@sha256:56b388b0d79c738f4cf51bbaf184a14fab19337f4819ceb2cae7d94100262de8
Deleted: sha256:11ceee7cdc57225711b8382e1965974bbb259de14a9f5f7d6b9f161ced50a10a
Deleted: sha256:509399ba28df5ec7538669d8d9da1d01bc8db8c7acbb2e93ab652535596ad63b
Deleted: sha256:59435c063da3dbad03d0decc30a79f187552d1af8e3e6ab3053f65b459ed5cec
Deleted: sha256:5f9e829c3d01da059a770adc5301b81f38d1bc32ac01a29cef77158d48c9e0f5
Deleted: sha256:10d6a41d302745409d3a2bfa711aa4ca5b815d09ce40c0dfafc676d93b901654
Deleted: sha256:859564a6de82045836ce2b228153e2314b14b1fd953f56ce94db723d66d2a4fa
Deleted: sha256:2e0710d2831319c131c54ad7b545e5089c1d111d45a95ade7f5ec106dc6d05d9
Deleted: sha256:72c690143394392f22d311d60d7b2cada541166fddd89ddf69d9564f3160e0fd
$ docker image ls
REPOSITORY   TAG       IMAGE ID   CREATED   SIZE
$