# RasCam
Transforms your Raspberry Pi into a security camera with management done from a remote server

##Why?
Why not? I was looking forward to do something with a Raspberry Pi and thought that a security camera would be a nice pet project and a great opportunity to learn something new.
Of course I had to do it in my own, twisted, way and here are the reasons:

1. **Security**. Other solutions requires that your device should be accessible from the Internet, so you can remotely stop the motion detection and see the images.
        If not properly configured, somebody can gain access to your Raspberry Pi and see everything. Uploading of the images to Dropbox only solves half of the problem.
        I my solution, the device only detects the movement and uploads the images to a remote server.
2. **Multiple cameras**. The server can manage and receive images from multiple cameras. Just configure another Raspberry Pi a voilà!
3. **Fun**. I really wanted to learn new technologies (for example [Docker](https://www.docker.com) and [AngularJS](https://angularjs.org) ) and have some fun.

The project is divided into 2 parts:

 - **[Client](https://github.com/SillentTroll/rascam_client)** part has all the code and installation scripts for Raspberry Pi.
 - **[Server](https://github.com/SillentTroll/rascam_server)** contains everything to setup and run the server code on your dedicated machine.

See each repo **README** file for installation and configuration steps.

##TODO
There are some things left to do:

 - Camera activation by schedule.
 - Notifications
 - Change [Motion](http://www.lavrsen.dk/foswiki/bin/view/Motion/WebHome) configs from the server.
  