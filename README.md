# hello2parikshit/docker-sigterm-trapping [![](https://images.microbadger.com/badges/image/hello2parikshit/docker-sigterm-trapping.svg)](https://microbadger.com/images/hello2parikshit/docker-sigterm-trapping "Get your own image badge on microbadger.com") [![](https://images.microbadger.com/badges/version/hello2parikshit/docker-sigterm-trapping.svg)](https://microbadger.com/images/hello2parikshit/docker-sigterm-trapping "Get your own version badge on microbadger.com")

To run the code, open a new terminal window and build the image for 30s sleep testing:

```
docker build -t hello2parikshit/docker-sigterm-trapping:30s .
```

Run the container:

```
docker run -it --rm -p 3000:3000 --name="signal-bg-app" hello2parikshit/docker-sigterm-trapping:30s
```
    
Get the process ID for container : 
    
```
$ docker ps

$ docker inspect <container_id> | grep -i pid
```
   
SIGTERM container process id :

```
$ sudo kill -s SIGTERM <pid>
```

Output : 

```
$ docker run -it --rm -p 3000:3000 --name="signal-bg-app" hello2parikshit/docker-sigterm-trapping
server started
^@server stopped by SIGTERM
sleeping 30s
sleeping done .. bye
```

Ref : https://medium.com/@gchudnov/trapping-signals-in-docker-containers-7a57fdda7d86
