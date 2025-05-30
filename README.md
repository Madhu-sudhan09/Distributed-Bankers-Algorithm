# Multi-User Banker's Algorithm Simulation

A C-based implementation of the Banker's Algorithm with advanced features including dynamic priority scheduling, deadlock prediction, resource borrowing, and distributed execution.

## Features

- Multi-user simulation with separate processes
- Classic Banker's Algorithm implementation
- Dynamic priority scheduling with aging
- AI-based deadlock prediction
- Resource borrowing between processes
- Distributed system simulation using TCP/IP
- Real-time monitoring

## Requirements

- GCC compiler
- POSIX-compliant system (Linux/Unix)
- pthread library
- Standard C libraries

## Building

To build the project, simply run:

```bash
make
```

This will create the `banker_simulator` executable.

## Running

To run the simulation:

```bash
./banker_simulator
```

## Project Structure

- `banker.h`: Core data structures and function prototypes
- `banker.c`: Implementation of the Banker's Algorithm
- `scheduler.c`: Priority scheduling and deadlock prediction
- `distributed.c`: Distributed system communication
- `main.c`: Main program and simulation logic

## Implementation Details

### Core Components

1. **Banker's Algorithm**
   - Maintains Available, Max, Allocation, and Need matrices
   - Implements safety algorithm
   - Handles resource requests and releases

2. **Priority Scheduling**
   - Dynamic priority assignment
   - Aging mechanism to prevent starvation
   - Priority-based resource allocation

3. **Deadlock Prediction**
   - Rule-based prediction system
   - Historical pattern analysis
   - Resource utilization monitoring

4. **Resource Borrowing**
   - Inter-process resource sharing
   - Safe borrowing protocols
   - Rollback mechanisms

5. **Distributed System**
   - TCP/IP-based communication
   - Message passing between nodes
   - Resource sharing across nodes

## Sample Data

The simulation includes three sample datasets for different users:

1. User 1: High resource requirements
2. User 2: Medium resource requirements
3. User 3: Low resource requirements

Each user has three processes with different priority levels and resource needs.

## Monitoring

The system provides real-time monitoring of:
- Current resource allocations
- Process states
- Priority levels
- Deadlock predictions
- Inter-node communications

## License

This project is open source and available under the MIT License. 