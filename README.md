# AppPerformanceAutoAnalysis
Application Performance Auto-Anaylysis.

# Performance Vector
CPU: sockets, cores, pinning...

NUMA: numa node topology, strategy...

Memory: size, swap...

Storage: iops, iobw...

Network: latency, bandwidth, interrupts...

Custom: scripts

# Performance Score
Score of standard/custom tools like dd, iperf, $(cat /tmp/app_score) and etc..

# Infrastructure
KVM with Libvirt

Docker

# Configuration Sample

    [strategy-plugin]
    available_strategy = controlled, random, full, target

    [static-vector]
    name = numa, memory, network, custom-variable

    [controlled-vector]
    name = cpu
    range
    step

    ...

# Report
RadarGraph

FlameGraph