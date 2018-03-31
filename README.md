# AndroidStudio-NoVNC
The main purpose of our project is to provide an application softwares all clients who do not have enough memory or the configuration to run these  softwares.

What we have done is
we created containerized softwares that can be run on any platform without any specific configuration.
Any one can run any application any time any where they want.
There is no need to install the software on your system. You can directly run the software on your browser .
This is a client server architecture project
A server will have all the running containers of softwares which uses the minimal space of your system.
Clients needs to do is type the server's ip on the browser and map the given port. They will get the running software instantly.

1. Pull this reporistory
2. cd /path/AndroidStudio-NoVNC

3.Firstly build the image using the Dockerfile

$ sudo docker build -t AndroidStudio-NoVNC .

4. Then run the conatiner using docker image.

$ docker run -p 8080:6080 -v /data:/data -d AndroidStudio-NoVNC 

5. Go to your browser and type
localhost:6080 or YOUR_SYSTEM'S_IP:6080

then
go to
Android-studio > bin > studio.sh or search in "opt" folder , then execute the script and run your android-studio on your browser
