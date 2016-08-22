robtimmer/syncthing
===================

[Syncthing](http://syncthing.net/) Docker image



    docker run -d \
        --name syncthing \
        --restart always \
        -p 8384:8384 -p 22000:22000 -p 21025:21025/udp \
        -v /opt/docker/syncthing/config:/home/syncthing/.config/syncthing \
        -v /opt/docker/syncthing/Sync:/home/syncthing/Sync \
        robtimmer/syncthing