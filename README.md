# Multi-threaded-Event-Reservation-System

This project involves the implementation of a concurrent event reservation system using POSIX threads (pthread). The system is designed to handle multiple operations, including booking, canceling, and querying event tickets, all executed concurrently by multiple worker threads. To ensure thread safety and proper synchronization among threads, the project employs mutexes and condition variables. These synchronization mechanisms help prevent race conditions and ensure that shared resources, such as event tickets, are managed correctly in a multi-threaded environment.
# Features
# Concurrency:
    The system can handle multiple threads (up to 20) performing operations simultaneously.
# Thread Safety:
    Mutexes (pthread_mutex_t) are used to ensure that shared data (such as the availability of seats) is accessed in a thread-safe manner.
# Synchronization: 
    Condition variables (pthread_cond_t) are used to synchronize threads, ensuring that operations on the same event do not conflict.
# Dynamic Seat Management:
    The system dynamically manages the booking and cancellation of seats, adjusting availability in real time.
