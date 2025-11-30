OS Lab Assignment 4 — System Calls, VM Detection & File System Operations

This repository contains Python, Bash, and C scripts that simulate core Operating System concepts such as system calls, process creation, IPC, batch execution, VM detection, and basic CPU scheduling.

Features Implemented
1. Batch Processing Simulation (Python)

Runs multiple Python scripts sequentially using:

subprocess.call(['python3', script])

2. System Startup & Logging

Simulates OS boot sequence using multiprocessing and logs:

Process start

Process termination

Creates: system_log.txt

3. System Calls & IPC

Implements:

fork()

exec()

wait()

Pipes (os.pipe())

Enables basic inter-process communication (parent → child).

4. VM Detection

Includes:

Shell script for system info (kernel, user, virtualization)

Python script to detect if system runs inside a VM

5. CPU Scheduling Algorithms

Simulates:

FCFS

SJF

Round Robin

Priority Scheduling

Computes Waiting Time (WT) and Turnaround Time (TAT).

How to Run
Run Python scripts
python3 scriptname.py

Run shell script
bash system_info.sh

Run C program
gcc ipc.c -o ipc
./ipc

Repository Structure
├── batch_runner.py
├── startup_logging.py
├── ipc_fork_exec.c
├── vm_check.py
├── system_info.sh
├── scheduling/
│   ├── fcfs.py
│   ├── sjf.py
│   ├── priority.py
│   └── round_robin.py
├── README.md

Learning Objectives

Understand system call behavior
Implement process creation & IPC
Simulate OS boot sequence
Detect virtual machine environments
Apply scheduling algorithms

Requirements

Python 3.x

GCC (for C program)

Linux / WSL recommended
