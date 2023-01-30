# Parallel programming in python
These are some python parallel programming examples. These examples all make use of the core.py file.

These examples are part of "Introduction to Concurrent Programming with GPUs" course.

* start_new_thread_example.py - This uses _thread to start threads that execute asynchronously from the test harness. Note that there are time.sleep calls to increase the probability that all threads will complete prior to the test harness exiting, though this is not guaranteed.
* threading_lock_acquire_release_example.py - This uses the Python 3 threading library to create a binary lock and a number of threads to independently use the lock to enter execution of a "critical" section of code.
* threading_semaphore_example.py - This uses the Python 3 threading library to create a semaphore (configured as either a binary or multiple use based on CLI arguments) and a number of threads to independently use the semaphore to lock execution of a "critical" section of code.