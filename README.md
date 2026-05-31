CPU Scheduling Simulator

A high-performance, low-level simulation engine built from scratch in C++. This project models core Operating System primitives, process state machines, and evaluates the algorithmic trade-offs of various CPU resource allocation strategies.


## Supported Scheduling Algorithms

1. **First-Come, First-Served (FCFS):** A non-preemptive algorithm that allocates the CPU based on process arrival order. Demonstrates the *Convoy Effect*.
2. **Shortest Job First (SJF):** A non-preemptive, greedy algorithm that selects the process with the shortest burst time next. Uses a Min-Heap/Priority Queue for an $O(\log n)$ process selection efficiency, minimizing average waiting time.
3. **Round Robin (RR):** A preemptive, time-sliced algorithm designed for fairness. Rotates processes using a circular ready queue based on a configurable **Time Quantum**, explicitly tracking context-switching overhead.