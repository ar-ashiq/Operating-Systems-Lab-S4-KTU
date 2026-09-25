# Operating Systems Lab - KTU S4

Programs and reference material for the Operating Systems laboratory in the fourth semester of the KTU CSE curriculum. The repository covers Linux commands, shell scripting, system calls, process scheduling, inter-process communication, synchronization, memory management, deadlocks, page replacement, and disk scheduling.

Every item below links directly to its source file on GitHub.

## Lab Programs

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

## Running the Programs

Compile C programs with a C compiler such as `gcc`:

```bash
gcc cycle5/fcfs.c -o fcfs
./fcfs
```

Run shell scripts with:

```bash
chmod +x cycle2/1grossSalary.sh
./cycle2/1grossSalary.sh
```

Some programs use POSIX system calls, shared memory, threads, or semaphores and may require a Unix-like operating system.

## Contributions

Found an issue or have an improvement? Please [open an issue](https://github.com/ar-ashiq/Operating-Systems-Lab-S4-KTU/issues) or submit a pull request. You can also contact [ashiqar2002@gmail.com](mailto:ashiqar2002@gmail.com).
