https://hub.docker.com/r/dorowu/ubuntu-desktop-lxde-vnc


# construir
docker build -t chemi_vnc_final . 

# arrancar

docker run -p 6080:80 -p 5900:5900 -v /dev/shm:/dev/shm chemi_vnc_final
