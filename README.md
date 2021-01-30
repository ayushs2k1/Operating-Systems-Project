# Road Construction Using Highway Planning and Obstruction Prevention

### Table Of Contents

-  Abstract
-  Introduction
-  Project Requirements
-  Literature Survey
-  Block Diagram
-  Pseudo Code
-  Output Screentshot
-  Conclusion
-  References
-  Our Team


### 1. Abstract

The project titled ROAD CONSTRUCTION USING HIGHWAY PLANNING AND
OBSTRUCTION PREVENTION aims to address one of the major issues that the Indian
road construction department is facing. These days we notice that a large number of roads
are not in proper condition and many of them require restoration. Many of which are in
high usage and require immidiate repair. Our project aims to help athorities with
providing them the most profitable path for road contruction for a given map and the
sequence in which these roads can be addressed so that it would be convenient for both
the authorities as well as the general public.Our project collects various forms regarding
the map for the road that needs to be constructed, with this data we find the most shortest
and profitable path possible . Then we collect data for utility and traffic for all the roads
,then we normalize the data collected and generate a appropriate sequence in which the
road construction should be addressed. We have also included a deadline section so that
the roads that take more then the allocated time are highlighted and if necessary removed.
Also, a check for hindrance detection is added which can be used when we have limited
number of resources and a proper allocation of these resources is required. For this we
take inputs for resources which can refer to asphalt, machinery, mortar etc. Then we
require maximum resources needed for each road, amount of resources allotted for each
road, and available resources, based on which a safe sequence is generated that prevents
any unwanted stoppage of work.


### 2. Introduction

In countries like India where we are seeing a steep rise in the overall population there arise a
necessity of new habitat and scouring of vacant land to make new buildings, accommodations
and environments which are connected by roads. As per the statistics we get to know that a
total of 2098624 km of road was laid in India alone during the period 2001 to 2005 and these
numbers are continuously rising with each passing year. So the maintenance and construction
of new roads require a tremendous work force and attention from the government. So it
becomes necessary to design a proper algorithm that can manage the overall process of road
construction.

So the first part of the project deals with the task of getting the parameters through which a
road can be assigned a particular priority and accordingly can be used for further estimations
and calculations. So for this purpose we consider 3 parameters associated with a particular
road namely the size,utility and the traffic associated with each road . For the purpose of
getting the road size we employ yet another renowned and precise algorithm known as
djikstra algorithm to get the shortest road length

Scheduling is one of the most widely used techniques to using which any operation involving
several tasks can be ordered in such a way so that easy execution of the entire operation
becomes possible in the most efficient way possible avoiding any sort of errors and
confusions. The programme that does the task of scheduling is termed as a scheduler. Now
the scheduling used in the project involves priority scheduling without the use of pre-
emption(the reason for the same is explained in the later part of the project) ,So here the
algorithm decides how to schedule the various construction processes in the given region
based on their priorities , which in-turn is decided on the basis of various factors which are
mentioned in the above paragraph of the project. So all the constructions will be handled
accordingly.

In the second part of the proposed work, We tried to focus on the very common issue of delay
and stopping of the entire construction process due unavailability of various resources
involved in the construction process so we compared this scenario with the dead-lock
condition that arises in the operating systems while assigning resources to various running
processes and this lead us to use the same algorithm that we use in operating systems that is
the bankers algorithm for our project as well using various resources involved in the road
construction process so as to avoid any condition of an absolute deadlock state in our
construction process. The resources we use are discussed in later part of the project .So using
this bankers algorithm we make sure that at no situation should occur where for the lack of
required resources, all work gets stopped or hindered. So, the implementation of this
algorithm becomes necessary. The safe sequence advices in what order to proceed so that by
the available resources, all tasks can be completed.


### 3. Project Resource Requirement

- Software Requirements
  
    This project has been created using CODE BLOCKS
C Programming language has been used for the code

- Hardware Requirements

    Intel i3/i5/i7/i9

    Windows 7/8/8.1/10

    4 GB RAM

    4.0 GHz processor
    

### 4. Literature Survey

- 1.Title : A Comparative Review of CPU Scheduling Algorithms
AUTHORS- Mohd Shoaib and Mohd Zeeshan Farooqui
  
  - CONFERENCE PAPER Conference: Proceedings of National Conference on Recent
      Trends in Parallel Computing (RTPC - 2014)
  - At: Aligarh, India

  Published in November 2014

ADVANTAGES: CPU Scheduling decides which tasks are to be ordered in what way so
that a particular algorithm is followed to queue the processes.
DISADVANTAGES:There is no involvement of premptive SRTF in the paper , the
comparision is done only considering the non preemptive SRTF

- 2.Title : A Comparative Study of CPU Scheduling Algorithms
AUTHORS: Neetu Goel ,Dr. R.B. Garg
 
  - Journal: International Journal of Graphics & Image Processing IJGIP [ VOL-2 , Issue-
4],
  
  Published in November 2012

ADVANTAGES: This research paper shows that First Come First Serve (FCFS) &
Shortest Job First (SJF) is generally suitable for batch operating systems and Round
Robin (RR) & Priority Scheduling (PS) is suitable for time shaing systems.

DISADVANTAGES: No new algorithm was proposed in this paper

- 3.Title: Design and Implementation of Multi parameter Dijkstra’s Algorithm: A Shortest
path algorithm for real road networks.
AUTHORS: Nishtha Kesswani, Dinesh Gopalani

  - Journal: International Journal of Advances in Engineering and Research [Volume 2,
Issue 3],

  Published in september 2011

ADVANTAGES: Taking the real road networks into consideration, this paper suggests a
modification of Dijkstra's algorithm, the multi-parameter Dijkstra’s algorithm (MPD) that
considers multiple parameters into consideration. Apart from the distance between any
two nodes, it considers factors such as time taken to travel from the source to the destination, 
congestion of the route etc. so that the user can select the desired route based
on his/her preferences.

DISADVANTAGES: Cosiderable importance was not given to traffic and utility of roads

- 4.Title: Performance of deadlock avoidance algorithms in flexible manufacturing systems.
AUTHORS: Maria P. Fanti,Bruno Maione,Saverio Mascolo,Biago Turchiano

  - Journal: Journal of Manufacturing Systems(Elsevier) [Volume 15, Issue 3]

  Published in 1996

ABOUT: This paper compares performances of some deadlock avoidance policies. First,
theoretical analysis is carried out by introducing a criterion for ordering different policies by
flexibility in resource allocation. Second, avoidance policies are applied to some case
studies, which are simulated in detail. The simulation analysis confirms the theoretical
results showing that the algorithms allowing larger flexibility in resource allocation lead to
better performance indices.

- 5.Title: Approaches for Deadlock Detection and Deadlock Prevention for Distributed
Systems.
AUTHORS: Dhiraj Gupta, V.K Gupta (Department of Computer Science,NIMS
University,Jaipur,Rajasthan, India

  - Journal: Res. J. Recent Sci., Volume 1, Issue (ISC-2011)

  Published in 2011

ABOUT: This paper, discusses about deadlock detection techniques and present
approaches for detecting deadlocks in Distributed Systems. In many other aspects of
distributed systems, they are harder to detect, avoid, and prevent. Deadlocks are a
fundamental problem in distributed systems. Deadlock detection is more difficult in systems
where there is no such central agent and processes may communicate directly with one
another.
- 6.Title: A Review Study on the CPU Scheduling Algorithms.
AUTHORS: Shweta Jain(Department of Computer Science, Shri R.G.P. Gujarati
Professional Institute) , Dr. Saurabh Jain(Institute of Computer Applications, Shri Vaishnav
Vidyapeeth Vishwavidyalaya)

  - Journal: International Journal of Advanced Research in Computer and
    Communication Engineering IJARCCE [Vol. 5, Issue 8]

  Published in August 2016

ABOUT: In this paper, a review of techniques proposed by different authors are discussed
which is helpful to design Operating Systems and new researches in Scheduling. System
designers have many complex decisions that they are required to make before finalizing
their designs. The selections of the appropriate processor scheduling algorithms allow them
to tailor the design to perform at the highest level of performance, reducing overall idle
time. Design specifications will drive decisions such as responsiveness, preemption, and
reliability. These combinations can benefit both single processor and multiprocessor
systems if selected in the proper combination.

- 7.Title: Research on the optimization of Dijkstra’s Algorithm and its application.
AUTHORS: Arjun RK, Pooja Reddy, Shama, M.Yamuna

  - Journal: International Journal of Science, Technology & Management IJSTM [Vol. 4,
Issue 1]
  
  PUBLISHED IN APRIL 2015

ABOUT: This paper mainly studied the application of the shortest path algorithm based on
the data structure, and proposed the improved Dijkstra’s algorithm, which optimized
selection of the shortest path node and data storage structure and organization. Studies
showed that, compared with the traditional Dijkstra’s algorithm, the optimized Dijkstra’s
algorithm which has optimized the space complexity, time complexity and storage
combination reduced the storage space, reduced data redundancy and greatly improved the
running rate. It was clearly shown that the optimized algorithm is more applicable to
calculate the shortest path.


### 5. Block Diagram

