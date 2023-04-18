---
toc: true
comments: true
layout: post
title: Computers and Networks (Unit 4)
description: Add Definitions from Unit 4 Computer Systems and Networks
---

## Requirements
> Work through College Board Unit 4... blog, add definitions, and pictures.  Be creative, for instance make a story of Computing and Networks that is related to your PBL experiences this year.


### How a Computer Works
> As we have learned, a computer needs aa program to do something smart.  The sequence of a program initiates a series of actions with the computers Central Processing Unit (CPU). This component is essentially a binary machine focussing on program instructions provided.  The CPU retrieives and stores the data it acts upon in Random Access Memory (RAM). Between the CPU, RAM, and Storage Devices a computer can work with many programs and large amounts of data.

List specification of your Computer, or Computers if working as Pair/Trio
- Processor GHz: Jishnu - 3.20 GHz, 
- Memory in GB: Jishnu - 15.7 GB, 
- Storage in GB: Jishnu - 477 GB, 
- OS: Jishnu - Windows 11, Alan - Windows, Tirth - Windows

Define or describe usage of Computer using Computer Programs. Pictures are preferred over a lot of text.  Use your experience.

Team Infographic:
![]({{site.baseurl}}/images/1.png)
![]({{site.baseurl}}/images/2.png)
![]({{site.baseurl}}/images/3.png)

Personal Definitions:
- Input devices: Hardware thing that the user can interact with in order to send data to the computer

Examples: Keyboard, Mouse, Mic, Camera, Touchscreen, e.t.c. 

- Output devices: Converts or transfers data from a computer to a user friendly way 

Examples: Screen Display changing, Speakers, Headphone, Printer, Touchscreen, e.t.c.

- Program File: File that contains a program with instructions for the computer to follow and execute

Examples: Google, Brave, Steam, Microsoft, e.t.c.

- Program Code: The code that has the instructions/steps for a program to follow

Examples: My Create Performance Task, this file and all the code in it, e.t.c.

- Processes: A running program on a device 

Examples: Vscode, Chrome, e.t.c.

- Ports: Endpoints for communication in a computer network

Examples: 4000, 5900, e.t.c.

- Data File: A computer file that contains a database or data (can be images, videos, and texts)

Examples: the sql database we made, the lottery data me and alan made before, the data.csv file

- Inspect Running Code: Run and Debugging a file to find out errors by going 1 by 1 or stopping certain parts of the code

Examples: VScode Run and Debug and breakpoints, Inspect in google pages 

- Inspect Variables: Setting breakpoints at certain parts of code and observing the code line by line seeing how different variables are being affected

Examples: VScode debug


### The Internet
> Watch/review College Board Daily Video for 4.1.1

- Essential Knowledge
    - A computing device is a physical artifact that can run a program. Some examples include computers, tablets, servers, routers, and smart sensors.
    - A computing system is a group of computing devices and programs working together for a common purpose.
    - A computer network is a group of interconnected computing devices capable of sending or receiving data.
    - A computer network is a type of computing system. 
    - A path between two computing devices on a computer network (a sender and a receiver) is a sequence of directly connected computing devices that begins at the sender and ends at the receiver.
    - Routing is the process of finding a path from sender to receiver.
    - The bandwidth of a computer network is the maximum amount of data that can be sent in a fixed amount of time.
    - Bandwidth is usually measured in bits per second

- Complete Vocabulary Matching Activity.  Incorporate this into your learnings from year.  To analyze measure path and latency use `traceroute` and `ping` commands from Linux Terminal.  
    - Path - a 
    - Route = e
    - Computer System - b
    - Computer Device - c 
    - Bandwidth - d
    - Computer Network - f

> Watch/review College Board Daily Video 4.1.2

- Complete True of False Questions
1. True, because open protocols enable greater freedom in sharing information across the internet
2. False, because the IETF establishes internet standards but does not restrict access to the internet by manufacturers or individuals
3. False, because the availability of MAC addresses is determined during file transfer, leading to different routes for transmission
4. True, because Internet Protocol and other protocols establish specific behaviors within the system through agreed-upon rules
5. False, because although UDP can provide faster transfer speeds, it does not guarantee consistent transfer success
6. False, because the World Wide Web is not the internet but functions by linking individual web pages
7. True, because HTTP is the protocol utilized by the World Wide Web to present website pages

- Essential Knowledge
    - The internet is a computer network consisting of interconnected networks that use standardized, open (nonproprietary) communication protocols.
    - Access to the internet depends on the ability to connect a computing device to an internet connected device.
    - A protocol is an agreed-upon set of rules that specify the behavior of a system.
    - The protocols used in the internet are open, which allows users to easily connect additional computing devices to the internet.
    - Routing on the internet is usually dynamic; it is not specified in advance
    - The scalability of a system is the capacity for the system to change in size and scale to meet new demands.
    - The internet was designed to be scalable
    - Information is passed through the internet as a data stream. Data streams contain chunks of data, which are encapsulated in packets. 
    - Packets contain a chunk of data and metadata used for routing the packet between the origin and the destination on the internet, as well as for data reassembly.
    - Packets may arrive at the destination in order, out of order, or not at all
    - IP, TCP and UDP are common protocols used on the internet.
    - The world wide web is a system of linked pages, programs, and files.
    - HTTP is a protocol used by the world wide web
    - The world wide web uses the internet

- Go over AP videos, vocabulary, and essential knowledge.  Draw a diagram showing the internet and its many levels. A preferred diagram would using your knowledge of frontend, backend, deployment, etc.  Picture would highlight vocabulary by illustration. The below illustration have some ideas

![]({{site.baseurl}}/images/FullStack_1.png)

- Often we draw pictures of machines communicating over the Internet with arrows.  However, the real communication goes through protocol layers and the machine and then is transported of the network.   For College Board and future Computer Knowledge you should become familiar with the following ...

```
     User Machine  <---> Frontend Server <---> Backend Server
    +-----------+         +-----------+         +-----------+
    |  Browser  |         |  GH Page  |         |   Flask   |
    +-----------+    ^    +-----------+    ^    +-----------+
    |    HTTP   |    |    |    HTTP   |    |    |    HTTP   |
    +-----------+    |    +-----------+    |    +-----------+
    |    TCP    |    |    |    TCP    |    |    |    TCP    |   
    +-----------+    |    +-----------+    |    +-----------+
    |     IP    |    V    |     IP    |    V    |     IP    |
    +-----------+         +-----------+         +-----------+
    |  Network  |  <--->  |  Network  |  <--->  |  Network  |
    +-----------+         +-----------+         +-----------+
```

The "http" layer is an application layer protocol in the TCP/IP stack, used for ***communication between web browsers and web servers***. It is the protocol used for transmitting data over the World Wide Web.

The "transport" layer (TCP) is responsible for providing reliable data transfer between applications running on different hosts.  The TCP protocol segments the data into smaller ***chunks called "segments"***. Each segment contains a sequence number that identifies its position in the original stream of data, as well as other control information such as source and destination port numbers, and checksums for error detection.

The "ip" layer is responsible for packetizing data received from the TCP layer of the protocol stack, and then ***encapsulating the data into IP packets***. The IP packets are then sent to the lower layers of the protocol stack for transmission over the network.

The "network" layer is responsible for ***routing data packets between networks*** using the Internet Protocol (IP). This layer handles tasks such as packet addressing and routing, fragmentation and reassembly, and ***network congestion*** control.


### Fault Tolerance
> Watch both Daily videos for 4.2

- Complete the network activity, summarize your understanding of fault tolerance.
1st Video for 4.2 Practice:

1. Yes, it is fault tolerant because even if one path goes down, you can communicate with the other ones due to the other connections it has
2. No, it isn't fault tolerant because there was only one path to F so if one wire goes down F is also cut off from the rest of the computers
3. No, it isn't fault tolerant because there is only one path connecting A and G and without G, A can't communicate with the rets of the computers

2nd Video for 4.2 Practice:
1. C
2. A, the internet is an fault tolerant network where devices can communicate with each other even if one path is down, there are multiple paths that can be used to transport information from one computer to another computer so information can be sent even if one path is down while its being repaired. The more paths a unit has, the more it would cost.



### Parallel and Distributed Computing
> Review previous lecture on Parallel Computing and watch Daily vidoe 4.3.  Think of ways to make something in you team project to utilize Cores more effectively.  Here are some thoughts to add to your story of Computers and Networks...

- What is naturally Distributed in Frontend/Backend archeticture?  

The backend is naturally distributed as it typically consists of multiple servers that can handle different tasks and by distributing them, they can take in a lot more requests at a single time. Frontend on the other hand is usually executed from a single device as its only interacting with the user.

- Analyze this command in Docker: ```ENV GUNICORN_CMD_ARGS="--workers=1 --bind=0.0.0.0:8086"```.   Determine if there is options are options in this command for parallel computing within the server that runs python/gunicorn.  Here is an [article](https://medium.com/building-the-system/gunicorn-3-means-of-concurrency-efbb547674b7)

This command is used to configure the Gunicorn web server. The –workers option specifies the number of worker processes that Gunicorn should spawn to handle incoming requests. In this case, the value is set to 1, which means that Gunicorn will use a single worker process to handle all requests meaning that it wouldn't be able to handle parallel computing since there is only one worker to process everything

> Last week we discussed parallel computing on local machine.  There are many options.  Here is something to get parallel computing work with a tool called Ray.
- Review this [article](https://www.anyscale.com/blog/writing-your-first-distributed-python-application-with-ray)...  Can you get parallel code on images to work more effectively?  I have not tried Ray.

Ray is a tool that helps you write Python programs that run faster by running them on multiple processors, GPUs, or machines at the same time

- Code example from ChatGPT using squares.  This might be more interesting if nums we generated to be a lot bigger.

```python
import ray

# define a simple function that takes a number and returns its square
def square(x):
    return x * x

# initialize Ray
ray.init()

# create a remote function that squares a list of numbers in parallel
@ray.remote
def square_list(nums):
    return [square(num) for num in nums]

# define a list of numbers to square
nums = [1, 2, 3, 4, 5]

# split the list into two parts
split_idx = len(nums) // 2
part1, part2 = nums[:split_idx], nums[split_idx:]

# call the remote function in parallel on the two parts
part1_result = square_list.remote(part1)
part2_result = square_list.remote(part2)

# get the results and combine them
result = ray.get(part1_result) + ray.get(part2_result)

# print the result
print(result)

```
