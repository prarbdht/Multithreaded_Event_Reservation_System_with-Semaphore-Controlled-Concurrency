# Multithreaded_Event_Reservation_System_with-Semaphore-Controlled-Concurrency

# Overview
This project implements a multi-threaded event-reservation system using pthread API and Grand Central Dispatch (GCD) for semaphore management. It is designed to manage up to 100 events with a capacity of 500 seats each, handling up to 20 concurrent threads and 5 active queries.

# Features
* Concurrency Management: Limits active queries using semaphores to ensure system stability.
* Mutual Exclusion: Uses mutexes to maintain data consistency, allowing only one write operation per event at a time.
* Dynamic Query Handling: Supports automatic generation and processing of queries for seat booking, cancellation, and availability checks.
* Performance Monitoring: Efficiently manages load and synchronizes thread operations.

# Requirements
* Operating System: Unix-based systems (including Linux distributions like Ubuntu and macOS)
* Libraries: pthread, GCD (dispatch)
* Compiler: GCC or Clang

# Installation
Clone the repository:

```Copy code
git clone https://github.com/yourusername/event-reservation-system.git
```
Navigate to the project directory:

```Copy code
cd event-reservation-system
```
Compile the project:

```Copy code
g++ -o event_reservation_system main.cpp -lpthread
```
# Usage
Run the program:

```Copy code
./event_reservation_system
```
Follow the prompts to input parameters:

Number of events
Capacity of each event
Number of worker threads
Maximum number of concurrent active queries
Total running time in seconds
The system will automatically generate and process queries, displaying the results in the console.

# Example
```plaintext
Enter the number of events: 100
Enter the capacity of auditorium: 500
Enter the number of worker threads: 20
Enter the maximum number of concurrent active queries: 5
Enter the total running time in seconds: 60
```

