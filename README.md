# Systems Programming Projects

A collection of systems programming projects in C and C++ exploring operating system concepts, process management, concurrency, inter-process communication, and virtual memory.

## Overview

This repository brings together four projects focused on understanding how software interacts with the operating system at a low level. From building a command shell and implementing CPU scheduling to parallel execution with Pthreads and demand-paged ELF loading, each project explores a different aspect of systems programming.

## Projects

### 1. [SimpleScheduler](https://github.com/sulpboy/SimpleScheduler-Implementation)

A process scheduling system that coordinates job execution using separate processes, pipes, and Unix signals.

- Process creation and management using `fork()`
- Inter-process communication using pipes
- Process suspension and resumption using `SIGSTOP` and `SIGCONT`
- Timer-driven scheduling and execution statistics

**Technologies:** C, Unix system calls, signals, pipes

### 2. [SimpleMultithreader](https://github.com/sulpboy/SimpleMultithreader)

A lightweight, header-only C++ library for parallelizing loop-based computations using POSIX threads and lambda functions.

- One-dimensional and two-dimensional parallel loops
- Work distribution across multiple threads
- Thread creation and synchronization using Pthreads
- Execution-time measurement

**Technologies:** C++, C++11, Pthreads

### 3. [SimpleShell](https://github.com/sulpboy/SimpleShell)

A Unix shell that executes external commands, supports multi-stage pipelines, and maintains command execution history.

- Command execution using `fork()` and `execvp()`
- Pipeline communication using `pipe()` and `dup2()`
- Process synchronization using `waitpid()`
- Command history and execution-time tracking

**Technologies:** C, Unix system calls, process management, IPC

### 4. [SmartELFLoader](https://github.com/sulpboy/SmartELFLoader)

A demand-paged loader for compatible 32-bit ELF executables that loads memory pages as they are accessed during execution.

- ELF header and program-header parsing
- On-demand page allocation using `mmap()`
- Page fault handling using `SIGSEGV`
- Memory permissions using `mprotect()`
- Page fault, allocation, and internal fragmentation statistics

**Technologies:** C, ELF, virtual memory, signal handling

## Concepts Covered

- **Process Management:** Process creation, scheduling, execution, and synchronization
- **Concurrency:** Multithreading, parallel loop execution, and workload distribution
- **Inter-Process Communication:** Pipes and file descriptor redirection
- **Virtual Memory:** Demand paging, memory mapping, and page fault handling
- **Unix System Programming:** System calls, signals, and resource management

## Languages and Tools

- **Languages:** C, C++
- **Platform:** Unix/Linux
- **Tools and APIs:** GCC, GNU Make, POSIX system calls, Pthreads

---

Each project has its own repository with implementation details, build instructions, and usage examples.
