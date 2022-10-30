RTSP-Client-Server
======


Introduction
----

Streaming videos are ubiquitous on the web today. 
Initially designed for simple text/document-based transfers using protocols such as the HTTP, 
the internet is the platform on which streaming media is passed from one end of the world to another. To stream data across networks efficiently, the layers of the network stack must be enhanced with capabilities to transfer it efficiently while not congesting the network as a whole.
This project examines how media can be transmitted over the web using [Real Time Streaming Protocol](https://en.wikipedia.org/wiki/Real-time_Transport_Protocol)(RTSP) and [Real-time Transport Protocol](https://en.wikipedia.org/wiki/Real-time_Transport_Protocol)(RTP/RTCP).
<br>
Implemented a streaming video server and client that communicates using the Real-Time Streaming Protocol (RTSP) and sends data using the Real-time Transfer Protocol (RTP). Here, the task is to implement the client's RTSP protocol and the server's RTP packetization. We will provide you with code that implements the RTSP protocol in the server, the RTP de-packetization in the client, and takes care of displaying the transmitted video.


State diagram of client state
---- 
![image](https://user-images.githubusercontent.com/75716586/198874566-e02d5d51-1270-410c-8970-9957078849e1.png) 

Architecture
----
![image](https://user-images.githubusercontent.com/75716586/198874775-a2e86dc2-217b-4679-aee4-71a44b313513.png)

Running Client/Server Programs
----
    Open a terminal:
        python Server.py 1025

    Open another terminal:
        python ClientLauncher.py 127.0.0.1 1025 5008 video.mjpeg


Start the server with the command line
	
		python Server.py server_port
	
Note : choose a port > 1024

Open a new terminal

	Start the client with the command line
		
		python ClientLauncher.py server_host server_port RTP_port video_file
	
For more information 
----
https://gaia.cs.umass.edu/kurose_ross/programming/Python_code_only/VideoStreaming_programming_lab_only.pdf
