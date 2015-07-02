HPServer is a free, open-source light-weighted framework for concurrent networking software.

Traits of HPServer:
> object-oriented;

> high-performance;

> cross-platform, support windows & linux;

> event-driven;

> support I/O events, timer, and signals;

> support acceptor-connector pattern internally, which will faciliates your programming;

> support multithread;
HPServer is imepletment with the C++ language.
Currently HPServer supports epoll, select in the form of reactor pattern, and it intends to integrate
both windows IOCP, and linux EPOLL into the proactor pattern, which will be implemented in the next build.

Based on our test, server using HPServer can acheive 10K concurrent connections easily! and the programming model fairly simple.
