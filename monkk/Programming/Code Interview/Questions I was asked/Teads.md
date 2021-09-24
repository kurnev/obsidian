[[OSI]]

Context switch 
single threaded processes vs multithreaded (nodejs) for web servers:

bad single threaded:
 context switch might hurt when there a lot of process (tens of thousands), because modern CPU does not have much cores and it can switch fast between processess
 there is a limit in linux, which stops you from calling too much threads (60k?)
 
 nodejs event loop
 
 