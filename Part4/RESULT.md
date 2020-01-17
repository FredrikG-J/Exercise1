In python, integers can't be changed since they are are immutable, since the integer objects can be used under several names. The
  magic number therefore does not become 0. Only one thread is in execution at the same time.
In Go, this is posible as the answer becomes 0. With go (Go) we create a coroutine, and GOMAXPROCS changes the number of processors
  that are being used.
In C, the code seems unstable. By incrementing and decrementing 10^5 times and lower, the answer becomes 0. However, with the use of
  10^6 the magic number varies. By using pthread_create() the function starts a new thread in the calling
       process.
