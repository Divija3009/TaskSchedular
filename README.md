# Overview
TaskSchedular is a distributed, fault-tolerant multi-node task scheduling system built using C++17, gRPC, and OpenMP.
It enables a scheduler to assign computational tasks to multiple worker nodes in a networked environment, monitor their execution via heartbeat signals, and dynamically balance the workload based on system capacity.
This project demonstrates key distributed-systems concepts such as:
1. Task orchestration across heterogeneous nodes
2. Heartbeat-based failure detection and recovery
3. Parallel task execution within worker nodes
4. gRPC-based communication for scalable system coordination

# Build Instructions
```
# Clone the repository
git clone https://github.com/DivijaChoudhary/TaskMaster.git
cd TaskMaster

# Configure build with CMake
cmake -B build -S . -DCMAKE_TOOLCHAIN_FILE="C:/path/to/vcpkg/scripts/buildsystems/vcpkg.cmake"

# Compile the project
cmake --build build

```
## Start Scheduler Server and worker node
```
./build/scheduler_server
./build/worker_node
```


