# System-Design

## Overview of Scaling
- In client-server based system there is a client who sends requests to the server and then the client receives a response from the server accordingly but when the number of users/clients increases, the load on the server increases enormously which makes it difficult for the server to perform efficiently and hence becomes slow. Therefore, it is important to make the server scalable in a way such that the server capacity increases according to the increasing traffic without any sort of failure.


## Scaling : 

- Scaling is the process to expand the existing configuration (servers/computers) to handle a large number of user requests or to manage the amount of load on the server. 
- This can be done either by increasing the current system configuration (increasing RAM, number of servers) or adding more power to the configuration. Scalability plays a vital role in the designing of a system as it helps in responding to a large number of user requests more effectively and quickly.
- There are two ways to do scaling :    
    1. Vertical Scaling 
    2. Horizontal Scaling 

### Vertical Scaling
- It is defined as the process of increasing the capacity of a single machine by adding more resources such as memory, storage, etc. to increase the throughput of the system. No new resource is added, rather the capability of the existing resources is made more efficient. This is called Vertical scaling. Vertical Scaling is also called the Scale-up approach. 

#### Pros of Vertical Scaling:
1. It is easy to implement.
2. Reduced software costs as no new resources are added.
3. Fewer efforts required to maintain this single system.
#### Cons of Vertical Scaling:
1. Single-point failure (if a server fails then the whole service is stopped.)
2. Since when the system (server) fails, the downtime is high because we only have a single server
3. High risk of hardware failures



### Horizontal Scaling
- It is defined as the process of adding more instances of the same type to the existing pool of resources and not increasing the capacity of existing resources like in vertical scaling. This kind of scaling also helps in decreasing the load on the server. This is called <b>Horizontal Scaling</b>.Horizontal Scaling is also called the Scale-out approach. 
- In this process, the number of servers is increased and not the individual capacity of the server. This is done with the help of a <b>Load Balancer</b> which basically routes the user requests to different servers according to the availability of the server. Thereby, increasing the overall performance of the system. In this way, the entire process is distributed among all servers rather than just depending on a single server. 

#### Pros of Horizontal Scaling:
1. Fault Tolerance means that there is no single point of failure in this kind of scale because there are 5 servers here instead of 1 powerful server. So if anyone of the servers fails then there will be other servers for backup. Whereas, in Vertical Scaling there is single point failure.
2. Low Latency: Latency refers to how late or delayed our request is being processed.
3. Built-in backup.

#### Cons of Horizontal Scaling:
1. Not easy to implement as there are a number of components in this kind of scale.
2. Cost is high.
3. Networking components like, router, load balancer are required.