# znc - docker-compose to run znc

`git clone git@github.com:danzarov/znc.git`

`cd znc && mkdir znc-configs`

### Create the configs

```
docker run -it -v `pwd`/znc-configs:/znc-data znc --makeconf
```

### Spin up znc 

`HOST_PORT=59999 CONTAINER_PORT=60000 docker-compose up -d`

***make sure the HOST_PORT and CONTAINER_PORT match with the ports you specified creating the config above***
