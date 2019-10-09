
## Reading Notes for distributed system for profit and fun,chapter 1

### 以下是读distributed system for profit and fun的一些笔记

#### Why use distributed system in software sense but not hardware?

...1. To aviod add hardware complexity, since sometimes upgrading hardware is not a viable strategy for large scale computing.
...2. When adding new machines, we have to use distributed algorithm to efficiently copy datas around and coordinate computation tasks. At minimum cost.

* Focus in this text:
...1. disributed programming and system in DATA CENTERS.
...2. Explore the system design space rather than optimization specific design.

#### Goal: achieve Scalability and ...
* 1.Scalability: how to dealt with size issue? a more formal definition:is the ability of a system, network, or process, to handle a growing amount of work in a capable manner or its ability to be enlarged to accommodate that growth.
.... About size scalability, geographic scalability, admin scalability.
* 2. Two relevant aspects:
...1.Performance (and latency):
Performance is characterized by the amount of useful work accomplished by a computer system compared to the time and resources used. Which means to achive:

...2.




#### 一些不太理解的地方：
```
Computations primarily benefit from high-end hardware to the extent to which they can replace slow network accesses with internal memory accesses. The performance advantage of high-end hardware is limited in tasks that require large amounts of communication between nodes.
```
* How to evaluate the trade off between network accesses and internal memory accesses? Should I check on the memory acess pattern or the memory hireachy in CSAAPP?

* However, as I can see in the figure for performance vs cluster size, the high communication works indeed gain much higher performace vs light communication.

