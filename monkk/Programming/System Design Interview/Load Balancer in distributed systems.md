**Load Balancer**

Hardware (some special machines for high throuput) and software 

TCP load balancer simply reroutes packets without looking inside 
HTTP load balancers gets an HTTP req from a client, establishes a connection to a server and sends the requests to the server. Can look inside message and make decisions based on anything inside (Cookie, headers)

There are several algoritms to load blanace: round robin, least time on request for server, hashing algo...

Health checking all servers to know which one can be used and stop traffic if server is dead. 

It is a path between client and partitrioning services. 