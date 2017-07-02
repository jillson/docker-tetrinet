# docker-tetrinet
docker-compose artifacts to spin up gtetrinet client (in xrdp) and server
usage:
```
  docker-compose build
  docker-compose up
  rdesktop 127.0.0.1:5556
    Inside rdesktop, login as foo, password bar, start gtetrinet client, point at server (docker-compose should say the name)
```  
TODO: drop a shortcut to gtetrinet on the user's desktop
