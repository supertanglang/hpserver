1. timer test:
> timer number: 32768
> pricision: < 10ms

2. stress test:
> the test program simulates an echo server to receive messages from clients,
> and a client simulator to issue a number of connections to the server and send messages.
> (see the source code of test-threads in the test)

> I/O method:                epoll
> server:                    1 accept thread, and 4 worker threads
> client simulation:         1 thread
> simulation client number : >= 20480, that's means that the program handles more than 20480\*2 sockets in the test.

test environment:
> Linux 2.6, redhat, 2G memory; CPU: Intel Pentinum(R) Dual-Core 2.4G;

The test isn't a stress test, but it shows that HPServer can easily handle C10K concurrent connections with a fairly simple programming model.