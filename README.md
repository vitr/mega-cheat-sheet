### Mega Cheat Sheet

[Docker Cheat Sheet](https://github.com/wsargent/docker-cheat-sheet) https://github.com/wsargent/docker-cheat-sheet  

    curl -sSL https://get.docker.com/ | sh
    sudo service docker restart


stop/remove all containers  

    
    docker kill $(docker ps -q)
    docker rm $(docker ps -a -q)
    docker rmi $(docker images -q -f dangling=true) 
    
    docker volume ls -qf dangling=true | xargs -r docker volume rm
    
    

more here https://www.calazan.com/docker-cleanup-commands/  
    
    
Remove all untagged images

In the process of running docker I had accumulated several images that are not tagged. To remove these I use this command:

`docker rmi $(docker images | grep "^<none>" | awk "{print $3}")`


ssh docker@$(boot2docker ip)
(password: tcuser, see https://github.com/boot2docker/boot2docker#ssh-into-vm)  
```
cat ~/.ssh/id_rsa.pub | ssh docker@$(boot2docker ip) 'cat - >> ~/.ssh/authorized_keys; chmod 600 ~/.ssh/authorized_keys'
```
and here is already added key `c:\Users\New\.docker\machine\machines\default\id_rsa`



Caddy - The HTTP/2 Web Server with Fully Managed SSL https://caddyserver.com/

    setcap cap_net_bind_service=+ep ./caddy


### PHP

Composer Cheat Sheet for developers http://composer.json.jolicode.com/

### Github

        git config --global credential.helper store

store username&password in `~/..git-credentials`
