COMPX234 - Lab Assignment 2
 
Readers-Writers Problem using a Monitor in Python
 
Project Description
 
This project implements the classic Readers-Writers problem using a monitor-style solution in Python.
The solution uses threading.Lock and threading.Condition to ensure safe concurrent access to a shared resource.
 
Rules enforced:
 
1. Multiple readers may read at the same time if no writer is writing.
2. A writer must have exclusive access.
3. Readers and writers cannot run at the same time.
 
How to Run
 
1. Make sure Python 3 is installed.
2. Run the program:
python readers_writers.py
 
Files
 
- readers_writers.py: Main implementation
- README.md: Documentation
 
Key Implementation
 
- ReadersWritersMonitor: Controls all synchronization
- start_read / end_read: Manage reader access
- start_write / end_write: Manage writer access
- Reader and Writer threads simulate concurrent access
 
Example Output
 
Reader 1 wants to read
Reader 1 starts reading. Active readers = 1
Reader 2 wants to read
Reader 2 starts reading. Active readers = 2
Reader 3 wants to read
Reader 3 starts reading. Active readers = 3
Writer 1 wants to write
Writer 2 wants to write
Reader 1 stops reading. Active readers = 2
Reader 2 stops reading. Active readers = 1
Reader 3 stops reading. Active readers = 0
Writer 1 starts writing
Writer 1 stops writing
Writer 2 starts writing
Writer 2 stops writing
 
All readers and writers have finished execution. Simulation completed.
 
Assignment Requirements Met
 
- Correct monitor with condition variables
- Multiple readers can read concurrently
- Writers have exclusive access
- At least 3 readers and 2 writers
- All threads started and joined properly
- Clear output messages
