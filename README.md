
# OS Algorithms Simulator in C

A command-line Operating Systems project that demonstrates two fundamental OS algorithms:

- **LRU (Least Recently Used) Page Replacement**
- **C-LOOK Disk Scheduling**

The project simulates how an operating system manages memory pages and services disk I/O requests. It displays the steps performed by each algorithm and reports useful performance metrics.

## Features

### 1. LRU Page Replacement

- Simulates page references using a fixed number of memory frames.
- Identifies page hits and page faults.
- Replaces the least recently used page when all frames are occupied.
- Displays the frame contents after each page reference.
- Calculates total page faults, page hits, and hit ratio.

### 2. C-LOOK Disk Scheduling

- Accepts a queue of disk track requests and an initial disk-head position.
- Sorts requests by track number.
- Services requests in the selected direction.
- Wraps around to the lowest pending request after reaching the highest request.
- Displays the head movement sequence.
- Calculates total seek distance and average seek distance.

## Technologies Used

- Programming Language: C
- Standard Libraries: `stdio.h`, `stdlib.h`
- Concepts: Arrays, structures, functions, sorting, page replacement, disk scheduling

## Project Structure

```text
os-algorithms-simulator/
├── lru.c
├── clook.c
├── README.md
└── .gitignore
```

## Requirements

- GCC or another compatible C compiler
- A terminal or command prompt
- Visual Studio Code is optional

## How to Run

### Step 1: Clone the repository

```bash
git clone https://github.com/Tejaswini-2310/os-algorithms-simulator.git
```

### Step 2: Open the project folder

```bash
cd os-algorithms-simulator
```

### Step 3: Compile and run LRU

```bash
gcc lru.c -o lru
```

On Windows:

```bash
lru.exe
```

On Linux or macOS:

```bash
./lru
```

### Step 4: Compile and run C-LOOK

```bash
gcc clook.c -o clook
```

On Windows:

```bash
clook.exe
```

On Linux or macOS:

```bash
./clook
```

## Sample Inputs

### LRU Page Replacement

Reference string:

```text
7 0 1 2 0 3 0 4 2 3 0 3 2
```

Number of frames:

```text
3
```

The program displays each page reference, whether it results in a hit or fault, the current frame contents, and the final performance statistics.

### C-LOOK Disk Scheduling

Request queue:

```text
98 183 37 122 14 124 65 67
```

Initial head position:

```text
53
```

The program displays the order in which requests are serviced, each head movement, the total seek distance, and average seek distance.

## Concepts Demonstrated

- Virtual memory and page replacement
- Page hits and page faults
- Least Recently Used replacement strategy
- Disk scheduling
- Seek distance and head movement
- Sorting and array manipulation
- Modular programming in C

## Future Improvements

- Add user input for reference strings and frame counts.
- Add validation for invalid page numbers and disk requests.
- Provide a menu to select an algorithm.
- Compare LRU with FIFO and Optimal page replacement.
- Compare C-LOOK with FCFS, SSTF, SCAN, and C-SCAN.
- Add graphical visualizations of frame states and disk-head movements.

## Learning Outcomes

This project provides practical experience implementing Operating Systems algorithms in C and understanding their execution through step-by-step console output.

## Author

**Tejaswini Kancharla**

- GitHub: https://github.com/Tejaswini-2310
- LinkedIn: https://linkedin.com/in/tejaswini-kancharla-845a55365

## Acknowledgment

If this project builds on work contributed by other developers, acknowledge the original repository and contributors here, and comply with the applicable license.
