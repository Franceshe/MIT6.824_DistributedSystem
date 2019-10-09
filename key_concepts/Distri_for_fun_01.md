
# Reading Notes for distributed system for profit and fun
## chapter 1

### 以下是读distributed system for profit and fun的一些笔记

### Why use distributed system in software sense but not hardware?

* To aviod add hardware complexity, since sometimes upgrading hardware is
not a viable strategy for large scale computing.
*  When adding new machines, we have to use distributed algorithm to efficiently copy datas around and coordinate computation tasks. At minimum cost.

### Focus in this text:
* disributed programming and system in DATA CENTERS.
* Explore the system design space rather than optimization specific design.

### Goal: achieve Scalability and ...
* Scalability: how to dealt with size issue? a more formal definition:is the
ability of a system, network, or process, to handle a growing amount of work in a capable manner or its ability to be enlarged to accommodate that growth.
* About size scalability, geographic scalability, admin scalability.
* Two relevant aspects:
... Performance (and latency)

### Some key concepts:
#### Performance
* Performance is characterized by the amount of useful work accomplished by a computer system compared to the time and resources used. Which means to achive:
... Short response time/low latency for a given piece of work
... High throughput (rate of processing work)
... Low utilization of computing resource(s)
* There's alwasys trade off between these factors, but low latency- - achieving a short response time - is the most interesting aspect of performance.

#### Latency:
* Intrinsicly:latency is the time during which something that has already happened is concealed from view.
* Extrinsic example: latency could be measured in terms of how long it takes for a write to become visible to readers.
* Diciding factor: speed of light which limits how fast "information" can travel and hardware components have a minimum latency cost incurred per operation.

#### Availability (and fault tolerance):
* Availability:
... the proportion of time a system is in a functioning condition. If a user cannot access the system, it is said to be unavailable.



#### 一些不太理解的地方：
```
Computations primarily benefit from high-end hardware to the extent to which
they can replace slow network accesses with internal memory accesses. The
performance advantage of high-end hardware is limited in tasks that require
large amounts of communication between nodes.
```
* How to evaluate the trade off between network accesses and internal memory
accesses? Should I check on the memory acess pattern or the memory hireachy in
CSAAPP?

* However, as I can see in the figure for performance vs cluster size, the high
communication works indeed gain much higher performace vs light communication.

