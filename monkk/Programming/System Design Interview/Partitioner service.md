It is a web service that gets requests from clients, looks inside eash request and routes to some partition. Partition is also a web service.  

**Hot partition** is a partition that takes a lot of requests. You can include event time to a partition key (if we select partition based on hashing algo )

**Service discovery** ZooKeeper

Each parition registers in zookeeper
server-side (load balancers) 
client-side

**Replication**
We must not lose events when we store 