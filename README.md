# Go-Loadbalancer
Bare-bones loadbalancer in Golang.
The load balancer uses the basic roundrobin solutions to 
distribute requests and this may have a drawback such as:

    Older nodes in the pool will always end-up processing more requests. Newly added nodes will end up processing less amount of traffic. If you instrumented auto-scaling in place, the problem gets even worse. In auto-scaling nodes are more dynamic. They get added and removed even more frequently.

There are a variety of load balancing algorithms we could use such as:

     Weighted Round Robin, Random, Source IP, URL, least connections, least traffic, and least latency.

But this project is a bare-bones project and those algorithms are beyond its scope.