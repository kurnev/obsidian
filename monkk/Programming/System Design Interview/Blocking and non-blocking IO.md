**Blocking IO**: one thread for a connection

They tend to be slower, but much easier to reason about. One thread per request, easier to debug by looking at a stack. 

**Non-blocking IO**: one thread handles all the requests and the actual request is processed later. They have better throughput as piling up request in a thread is way better, then piling up a lot of threads 