# hello2parikshit/docker-sigterm-trapping [![](https://images.microbadger.com/badges/image/hello2parikshit/docker-sigterm-trapping.svg)](https://microbadger.com/images/hello2parikshit/docker-sigterm-trapping "Get your own image badge on microbadger.com") [![](https://images.microbadger.com/badges/version/hello2parikshit/docker-sigterm-trapping.svg)](https://microbadger.com/images/hello2parikshit/docker-sigterm-trapping "Get your own version badge on microbadger.com")

To run the code, open a new terminal window and build the image:

    docker build -t hello2parikshit/docker-sigterm-trapping .

Run the container:

    docker run -it --rm -p 3000:3000 --name="signal-bg-app" hello2parikshit/docker-sigterm-trapping 


Ref : https://medium.com/@gchudnov/trapping-signals-in-docker-containers-7a57fdda7d86
