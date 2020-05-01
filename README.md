# hello2parikshit/docker-sigterm-trapping-background 

To run the code, open a new terminal window and build the image:

    docker build -t hello2parikshit/docker-sigterm-trapping-background .

Run the container:

    docker run -it --rm -p 3000:3000 --name="signal-bg-app" hello2parikshit/docker-sigterm-trapping-background 


Ref : https://medium.com/@gchudnov/trapping-signals-in-docker-containers-7a57fdda7d86
