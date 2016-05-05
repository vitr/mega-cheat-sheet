### Mega Cheat Sheet

[Docker Cheat Sheet](https://github.com/wsargent/docker-cheat-sheet) https://github.com/wsargent/docker-cheat-sheet  
stop/remove all containers  

    
    docker kill $(docker ps -q)
    docker rm $(docker ps -a -q)
    docker rmi $(docker images -q -f dangling=true) 

more here https://www.calazan.com/docker-cleanup-commands/  
    
    
Remove all untagged images

In the process of running docker I had accumulated several images that are not tagged. To remove these I use this command:

`docker rmi $(docker images | grep "^<none>" | awk "{print $3}")`





Caddy - The HTTP/2 Web Server with Fully Managed SSL https://caddyserver.com/

    setcap cap_net_bind_service=+ep ./caddy


### PHP

Composer Cheat Sheet for developers http://composer.json.jolicode.com/

### Github

        git config --global credential.helper store

store username&password in `~/..git-credentials`
