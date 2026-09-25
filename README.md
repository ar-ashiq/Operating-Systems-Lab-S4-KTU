# Operating Systems Lab - KTU S4

> A practical collection of **Operating Systems laboratory programs for KTU CSE S4**.

[![C](https://img.shields.io/badge/language-C-00599C?logo=c&logoColor=white)](https://en.wikipedia.org/wiki/C_(programming_language))
[![Shell](https://img.shields.io/badge/language-Shell-4EAA25?logo=gnu-bash&logoColor=white)](https://www.gnu.org/software/bash/)
[![GitHub stars](https://img.shields.io/github/stars/ar-ashiq/Operating-Systems-Lab-S4-KTU?style=social)](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU)

This repository brings together the source code and reference material completed during the Operating Systems lab. It is useful for revising concepts, preparing for practical examinations, and comparing different OS algorithms through small, readable implementations.

## What You Will Find

- Linux command reference material and shell scripting exercises
- UNIX process, directory, and file I/O system calls
- CPU scheduling simulations with waiting and turnaround times
- Shared-memory IPC and semaphore-based synchronization problems
- Fixed and variable partition memory allocation
- FIFO, LRU, LFU, and Optimal page replacement
- Banker's safety algorithm and deadlock detection
- FCFS, SCAN, and CSCAN disk scheduling

## Quick Navigation

| Topic | Start here |
| --- | --- |
| Shell scripting | [Cycle 2](#cycle-2---shell-scripting) |
| System calls and file I/O | [Cycles 3-4](#cycle-3---process-and-directory-system-calls) |
| CPU scheduling | [Cycle 5](#cycle-5---cpu-scheduling-algorithms) |
| IPC and synchronization | [Cycles 6-7](#cycle-6---ipc-using-shared-memory) |
| Memory management | [Cycles 8-9](#cycle-8---memory-allocation) |
| Deadlocks and disk scheduling | [Cycles 10-11](#cycle-10---deadlock-handling) |
| Complete file list | [Lab Programs](#lab-programs) |

## Lab Overview

| Cycle | Area | Main concepts | Files |
| --- | --- | --- | ---: |
| 1 | Linux commands | Command-line fundamentals | 1 |
| 2 | Shell scripting | Conditions, loops, search, patterns, arguments | 14 |
| 3 | System calls | `fork`, `exec`, `stat`, directory operations | 4 |
| 4 | File I/O | `open`, `read`, `write`, `close` | 1 |
| 5 | CPU scheduling | FCFS, SJF, SRTF, Round Robin, Priority | 5 |
| 6 | Shared-memory IPC | `shmget`, `shmat`, `shmdt`, `shmctl` | 3 |
| 7 | Synchronization | Semaphores and classic problems | 4 |
| 8 | Memory allocation | Fixed and variable partitions | 2 |
| 9 | Page replacement | FIFO, LRU, LFU, Optimal | 5 |
| 10 | Deadlock handling | Safety, resource requests, detection | 4 |
| 11 | Disk scheduling | FCFS, SCAN, CSCAN | 2 |

## Getting Started

### Prerequisites

You will need:

- A Unix-like operating system such as Linux or macOS
- GCC or another C compiler
- Bash or a compatible shell
- POSIX development support for programs using processes, threads, shared memory, or semaphores

### Clone the Repository

```bash
git clone https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU.git
cd Operating-Systems-Lab-S4-KTU
```

### Compile and Run a C Program

```bash
gcc cycle5/fcfs.c -o fcfs
./fcfs
```

For a program using POSIX threads or semaphores, your platform may require an additional linker flag:

```bash
gcc cycle7/producerConsumer.c -o producer_consumer -pthread
./producer_consumer
```

### Run a Shell Script

```bash
chmod +x cycle2/1grossSalary.sh
./cycle2/1grossSalary.sh
```

Most programs are interactive and expect input from the terminal. Read the source before running it so you know the expected input format and algorithm assumptions.

## Lab Programs

All links below open the corresponding file directly on GitHub.

### Cycle 1 - Linux Commands

- [Linux commands reference](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/blob/master/cycle1/osLab_linux_commands.pdf) - Reference questions and material for commonly used Linux commands.

### Cycle 2 - Shell Scripting

- [Gross salary](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/blob/master/cycle2/1grossSalary.sh) - Calculates gross salary using the given HRA and DA rules.
- [Armstrong numbers](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/blob/master/cycle2/2armstrong.sh) - Prints Armstrong numbers within an input range.
- [Smallest of three numbers](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/blob/master/cycle2/3smallest_of_3.sh) - Finds the smallest value among three inputs.
- [Password validation](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/blob/master/cycle2/4password_validate.sh) - Checks password length, letter case, digit, and underscore requirements.
- [Three-digit numbers](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/blob/master/cycle2/5_3digit_numbers.sh) - Generates three-digit numbers made from `0`, `1`, `2`, and `3`, without leading zeroes.
- [Palindromic prime](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/blob/master/cycle2/6palindromicPrime.sh) - Finds the smallest palindromic prime greater than a given number.
- [Sort numbers](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/blob/master/cycle2/7sort.sh) - Sorts a list of numbers using bubble sort.
- [Linear search](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/blob/master/cycle2/8linearSearch.sh) - Searches for an element in a list using linear search.
- [Number pattern](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/blob/master/cycle2/9pattern_1.sh) - Prints a repeated-number triangle for a specified number of rows.
- [Diamond pattern](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/blob/master/cycle2/10_diamond_pattern.sh) - Prints a star diamond pattern.
- [File names to uppercase](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/blob/master/cycle2/11fileToUppercase.sh) - Validates file arguments and displays existing file names in uppercase.
- [Reverse arguments](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/blob/master/cycle2/12Print_arguments_inReverse.sh) - Prints command-line arguments in reverse order.
- [Fibonacci](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/blob/master/cycle2/fibonacci.sh) - Computes a Fibonacci value for a given position.
- [Sum of digits](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/blob/master/cycle2/sumOfDigits.sh) - Displays the digits of a number and calculates their sum.

### Cycle 3 - Process and Directory System Calls

- [Fork, process IDs, exit, and wait](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/blob/master/cycle3/fork.c) - Demonstrates parent-child process creation and synchronization.
- [Exec](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/blob/master/cycle3/exec.c) - Replaces the current process with the `ls -l` command using `execlp`.
- [Stat](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/blob/master/cycle3/stat.c) - Reads file metadata such as size, device ID, and timestamps.
- [Directory operations](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/blob/master/cycle3/opendir.c) - Opens a directory, reads its entries, and closes it.

### Cycle 4 - File I/O System Calls

- [Open, read, write, and close](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/blob/master/cycle4/open_read_close.c) - Demonstrates basic file I/O system calls using [file.txt](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/blob/master/cycle4/file.txt).

### Cycle 5 - CPU Scheduling Algorithms

- [First Come First Served](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/blob/master/cycle5/fcfs.c) - Calculates scheduling results for non-preemptive FCFS.
- [Round Robin](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/blob/master/cycle5/roundRobin.c) - Simulates time-sliced scheduling with a configurable quantum.
- [Shortest Job First](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/blob/master/cycle5/sjf.c) - Implements non-preemptive SJF scheduling.
- [Shortest Remaining Time First](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/blob/master/cycle5/sjf_preemtive%28srtf%29.c) - Implements preemptive SJF scheduling.
- [Priority scheduling](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/blob/master/cycle5/Priority.c) - Implements non-preemptive priority scheduling.

### Cycle 6 - IPC Using Shared Memory

- [Shared-memory writer](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/blob/master/cycle6/ipc1.c) - Creates or attaches to shared memory and writes user input.
- [Shared-memory reader](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/blob/master/cycle6/ipc2.c) - Reads from shared memory and removes the shared-memory segment.
- [Shared-memory key file](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/blob/master/cycle6/shm) - File used as the `ftok` path/key source.

### Cycle 7 - Semaphores and Synchronization

- [Dining Philosophers](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/blob/master/cycle7/diningPhilosopher.c) - Coordinates philosophers competing for shared chopsticks.
- [Producer-Consumer](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/blob/master/cycle7/producerConsumer.c) - Synchronizes producers and consumers with counting semaphores and a mutex.
- [Readers-Writers](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/blob/master/cycle7/readersWriter.c) - Coordinates concurrent readers and exclusive writers.
- [Sleeping Barber](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/blob/master/cycle7/sleeping_barber.c) - Models waiting customers, barber availability, and limited waiting seats.

### Cycle 8 - Memory Allocation

- [Fixed-partition allocation](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/blob/master/cycle8/fixed_partition_allocation.c) - Compares First Fit, Best Fit, and Worst Fit for fixed partitions.
- [Variable-partition allocation](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/blob/master/cycle8/variable_partition_allocation.c) - Compares First Fit, Best Fit, and Worst Fit for variable partitions.

### Cycle 9 - Page Replacement Algorithms

- [FIFO page replacement](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/blob/master/cycle9/fifo.c) - Simulates FIFO replacement and counts page faults.
- [LRU page replacement](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/blob/master/cycle9/lru.c) - Replaces the least recently used page.
- [LFU page replacement](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/blob/master/cycle9/lfu.c) - Replaces the least frequently used page.
- [Optimal page replacement](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/blob/master/cycle9/Optimal.c) - Selects the page whose next use is farthest in the future.
- [Combined page replacement algorithms](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/blob/master/cycle9/all_page_replacementAlgos.c) - Menu-driven implementation of FIFO, LRU, and LFU.

### Cycle 10 - Deadlock Handling

- [Banker's algorithm](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/blob/master/cycle10/bankers.c) - Checks system safety and attempts to produce a safe sequence.
- [Safety algorithm](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/blob/master/cycle10/safetyAlgo.c) - Determines whether resource allocation can reach a safe state.
- [Safety algorithm with resource requests](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/blob/master/cycle10/safetyAlgoReq.c) - Tests a tentative resource request before granting it.
- [Deadlock detection](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/blob/master/cycle10/deadlockDetection.c) - Detects deadlocks using allocation, outstanding requests, and available resources.

### Cycle 11 - Disk Scheduling Algorithms

- [Disk scheduling](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/blob/master/cycle11/diskscheduling.c) - Simulates FCFS, SCAN, and CSCAN scheduling.
- [Extended disk scheduling](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/blob/master/cycle11/diskScheduling_extended.c) - Simulates disk scheduling with configurable head direction.

## Learning Path

1. Begin with [shell scripting](#cycle-2---shell-scripting) to practise input, conditions, loops, and functions.
2. Move to [system calls](#cycle-3---process-and-directory-system-calls) and [file I/O](#cycle-4---file-io-system-calls).
3. Compare the [CPU scheduling](#cycle-5---cpu-scheduling-algorithms) algorithms using the same process concepts.
4. Study [IPC and synchronization](#cycle-6---ipc-using-shared-memory) before working through deadlocks.
5. Finish with [memory management](#cycle-8---memory-allocation), [page replacement](#cycle-9---page-replacement-algorithms), and [disk scheduling](#cycle-11---disk-scheduling-algorithms).

## Contributions

Found an error, portability issue, or a missing lab program? Contributions are welcome.

1. Fork the repository.
2. Create a focused branch for your change.
3. Test the program on a Unix-like system.
4. Open a pull request with a short explanation of the change.

You can also [open an issue](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/issues) or contact [ashiqar2002@gmail.com](mailto:ashiqar2002@gmail.com).

## Acknowledgements

Created as a practical study resource for Kerala Technological University (KTU) Computer Science students learning Operating Systems.

## License

This repository is licensed under the [MIT License](LICENSE). You are free to use, modify, and distribute the programs with the license notice included.
