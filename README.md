# C-webserver
This is a very lightweight and simple HTTP server created for learning C, sockets, and HTTP RFC.
# A True Alpha Web Server in C
### Written By Xyconix
## Goals 
Here, we will be learning from a low-level (C), how web servers actually work, how they serve files, deliver files, and learn how the web works in general through a project-oriented/build-by-learning methodology.
### Promise to myself
Today's date is June 10th, 2024. I will complete this and make this a side project on top of the 1,000 other "pits" I have in the fire. But, I truly feel like this is important and want to increase my C skills.
## Motivation
The ultimate goal is to understand how a web server works at a very low level. First, we will need to understand how sockets work, which good thing we're pretty much there!
I believe that this will greatly enhance my current and future knowledge-base with CNO tooling development R&D-styled work. I hope you enjoy the adventure!
## Implementation
By utilizing and harnessing the power of libc, we can use the C standard library package, `<sys/socket.h>` to allow our program/server the ability to handle and form connections over the Internet.
This will be following a client/server model of course. The server will essentially be allowed to talk to our clients over a network or even the Internet by the end of this!
## Ideology:
	``` Server								Client
	    1. Create socket on port x			<---> TCP Connection Established <--->		1. Create socket & connect to server_IP:Port
	    2. Wait for incoming request from client				2. Send request 
	    3. Read request from client						3. Read reply
	    4. Write reply to client						4. Close socket
	    5. Close connection/socket```
