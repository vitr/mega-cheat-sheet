### Mega Cheat Sheet

[Docker Cheat Sheet](https://github.com/wsargent/docker-cheat-sheet) https://github.com/wsargent/docker-cheat-sheet  
stop/remove all containers  

    docker stop $(docker ps -q)
    docker rm $(docker ps -a -q)
    docker rm -f $(docker ps -a -q)

