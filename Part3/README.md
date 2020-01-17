# Reasons for concurrency and parallelism


To complete this exercise you will have to use git. Create one or several commits that adds answers to the following questions and push it to a repository to complete the task. Remember to also submit your answers to Blackboard

When answering the questions, remember to use all the resources at your disposal. Asking the internet isn't a form of "cheating", it's a way of learning.

 ### What is concurrency? What is parallelism? What's the difference?
Concurrency - multiple calculations overlap at the same time on a single
    prossessor. Parallelism - multiple calculations overlap at the same time on
    multiple prosessors. 
    
 ### Why have machines become increasingly multicore in the past decade?
- To be able to run more programs  in parallel, the machines has become
    increasingly multicore. 
    
 ### What kinds of problems motivates the need for concurrent execution?
 (Or phrased differently: What problems do concurrency help in solving?)
-  Data can be isolated through conflicting datachanges, and
    concurrency is used for this. 
    
 ### Does creating concurrent programs make the programmer's life easier? Harder? Maybe both?
 (Come back to this after you have worked on part 4 of this exercise)
    - Altering hte same program is easier.
 
 ### What are the differences between processes, threads, green threads, and coroutines?
- Thread: A set of instructions executed independently is called a thread. 
    - Process: A process is a computer program consisting of a thread or several
    threads.
    - Green thread: When something else than the OS is scheduling a
    thread. 
    - Coroutines: A general controll structure.
    
 ### Which one of these do `pthread_create()` (C/POSIX), `threading.Thread()` (Python), `go` (Go) create?
- Pthread_create() and Threading.thread() creates a thread
    - Go creates a coroutine.
 
 ### How does pythons Global Interpreter Lock (GIL) influence the way a python Thread behaves?
    - Lock GIL only allows one thread to be in execution at the same time
 
 ### With this in mind: What is the workaround for the GIL (Hint: it's another module)?
    - One can use extensions like Numpy.
 
 ### What does `func GOMAXPROCS(n int) int` change? 
    - This changes the number of processors that are being used.
