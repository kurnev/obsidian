1. Ask questions to clarify the requirements:
	1. users - who will use the system, how often
	2. scale (read and write) - how many read/write per request/second
	3. perf - write/read delay, is it real time. how fast 
	4. cost (budget) - technology stack, to minimize cost open source, maintenance
2. Write all functional requirements, write down API eaxmple 


[[Cap theorem]] should be kept in mind

Define a data model:
	**Individual events** 
		pros: are easy to write, manage and recalculate if needed
		cons: slow reads, costly for large scale 
	**aggregated data**
		pros: fast reads, data is ready
		cons: filtering and queiris are limited, impossible to fix errors
		
[[Big Data Stream data processing]]
[[Big Data batch data processing]]

We can also combine processing: store raw data for several days and then purge it. 

**Mysql:**
Mysql sharding is an option (horizontal scalability)
**Performance**: Probably behind the clust proxy with Configuration service (ZooKeeper) also with shard proxy for each shard.
**Availablity**:  read replica for a master shards on differenet data center


[[NoSQL]]

**Eventual consistency** - it takes time to propagate all changes to read replicas

For relaibality use replication and checkpointing
for fast use in-memory and minimize disk reads

**Data aggregation**

 We can pre-aggregate data in processing service or send it one-by-one. Usually aggregating is better for large-scale systems
 
 Push or pull ? 
 
 Pull provides better fault di
 
 For processing data: 
 
 [[Data aggregation Checkpointing]]
  
 [[Data aggregation Paritioning]]
 
 Processing service also may send to [[Dead letter queue]] in case when he can't reach the main database. And then another reader reads from it. 
 
**Data ingestion path:**

When user enters website he enters a API Gateway routes requests to backend systems.

[[Blocking and non-blocking IO]]

Load balancing may use batching to keep some data and send in one request, it has a lot of positives but has drawbacks: it introduces complexity both on client and the server side.

[[Load Balancer in distributed systems]]

 