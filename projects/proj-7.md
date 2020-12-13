---
layout: post
title: 'Introduction to Operating Systems'
---

Aug – Dec 2020

- I learnt about fundamentals of systems design while completing the projects for this <a href="http://omscs.gatech.edu/cs-6200-introduction-operating-systems" target="_blank"> class</a>.

- Specifically, I learnt how to  :
    <ul>
    <li> implement protocols for file transfer, using socket based API, between two multithreaded processes running on the same machine,</li>
    <li> implement protocols for file transfer, using shared memory based API, between two multithreaded processes running on the same machine, and</li>
    <li> implement remote procedure calls for file transfer in a distributed system.</li>
    </ul>

- **Tools used**: C, Valgrind, C++, gRPC, Protobuf, POSIX C API for multithreading,   <a href="https://www.man7.org/linux/man-pages/man7/shm_overview.7.html" target="_blank"> shared memory</a> and synchronization using semaphores

- **Theory concepts learnt**
    <ul>
        <li>Polices used by operating systems scheduler, such as,
            <ul> First Come First Serve, Shortest Job First, Round Robin </ul>
        </li>
        <li> Memory managment techiques like
            <ul>Paging and segmentation as well as caching policy using Least Recently Used(LRU) </ul>  
        </li>          
        <li> Virtualization concepts, models and techniques,
            <ul>Virtual Machine Monitor/ Hypervisor responsibilites, paravirtualization, OS protection rings and modes   </ul>
        </li>
        <li> Distributed File Systems and Distributed Shared Memory 
            <ul> consistency models such as sequential and weak, file sharing semantics like session based and periodic updates</ul>
        </li>
        <li> Cloud computing terminology 
            <ul> Infrastructure as a Service like Amazon EC2, Platform as a Service like Google App Engine, Software as a Service like Gmail</ul>
        </li>
    </ul>

**Selected Figures**    
{% include image_same_size.html image="projects/proj-7/
P3_reader_writer_sync_semaphore.png" %}

**Figure 1**: Flow of control diagram, between two processes using shared memory, to showing read-write sequence implemented using 
POSIX semaphores. Keyed off examples and notes <a href="https://man7.org/conf/lca2013/IPC_Overview-LCA-2013-printable.pdf" target="_blank"> here</a>.

{% include image_same_size.html image="projects/proj-7/P3_Cache_Service_Shared_memory.png" %}
**Figure 2**: Flow of control (a)between a client and web proxy via sockets 
and (b) between web proxy and a cache server using shared memory. CMQ in the figure represents a central message queue using POSIX API. SHM refers to Shared Memory.


{% include image_same_size.html image="projects/proj-7/
P4_Store_with_Lock_AFS.png" %}
**Figure 3**: Flow of Control diagram for Store command used in simple distributed file system. Locking for files prevents concurrent writes.