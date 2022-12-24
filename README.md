# System-Design

## Overview of Scaling
- In client-server based system there is a client who sends requests to the server and then the client receives a response from the server accordingly but when the number of users/clients increases, the load on the server increases enormously which makes it difficult for the server to perform efficiently and hence becomes slow. Therefore, it is important to make the server scalable in a way such that the server capacity increases according to the increasing traffic without any sort of failure.


## Scaling : 

- Scaling is the process to expand the existing configuration (servers/computers) to handle a large number of user requests or to manage the amount of load on the server. 
- This can be done either by increasing the current system configuration (increasing RAM, number of servers) or adding more power to the configuration. Scalability plays a vital role in the designing of a system as it helps in responding to a large number of user requests more effectively and quickly.
- There are two ways to do scaling :    
    1.Vertical Scaling <br />
    2.Horizontal Scaling 

### Vertical Scaling
- It is defined as the process of increasing the capacity of a single machine by adding more resources such as memory, storage, etc. to increase the throughput of the system. No new resource is added, rather the capability of the existing resources is made more efficient. This is called Vertical scaling. Vertical Scaling is also called the Scale-up approach. 

#### Pros of Vertical Scaling:
1. It is easy to implement.
2. Reduced software costs as no new resources are added.
3. Fewer efforts required to maintain this single system.
#### Cons of Vertical Scaling:
1. Single-point failure
2. Since when the system (server) fails, the downtime is high because we only have a single server
3. High risk of hardware failures