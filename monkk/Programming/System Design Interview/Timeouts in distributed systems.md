We can find 1% of slowest requests and set it as timeout, this way 1% of requests will fail. Retry those requeests for these requests. 

Also we can increase timeouts for each retry (exponentional backoff)
Jitter adds random time to these retries, so we do not overload our servers. 
Circuit breaker stops the requests from sending if there are too many. 