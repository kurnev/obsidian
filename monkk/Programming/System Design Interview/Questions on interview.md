Q: There is scheme of how SSPs (hunderds of them) work and they mostly write to the SQL database.  We know SQL is the bottleneck, so what we do to improve perf there.
A: Sharding is good, adding redis in front of sql. Feeder (process that fill redis from SQL). Add in-memory cache to SSP. Add communication between SSP process, so they could fill the cache if some outage happens to decrease the delay

Q: What would you do to get logs from SSPs
A: I would ooutput them based on 12factorapp to stdout. There will be a process that will collect those logs. They can later be put in Apache Cassandra and processed in Kafra beforehand. It is good to do a rollup of logs. We can keep old logs on some S3.  
 
 
 Read about AWS . 