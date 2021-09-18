Runs on [[graphs]]. Answers two questions:

1: Is there a path from node A to node B?
2: What is the shortest (fewest segments) path from node A to node B?

First search closest nodes. 

You need to check in the same order people were added to the search list to get shortest path. Don't check same node twice - check

Start from one node and add all his nodes to the queue. Pop the queue and check the item, if found - exit, if not found add all his nodes to the list.

def search(name):  
	search_queue = deque()  
	search_queue += graph[name]  
	searched = []
	while search_queue:  
		person = search_queue.popleft()  
		if not person in searched: 
			if person_is_seller(person):  
				print person + “ is a mango seller!”  
				return True  
			else:  
				search_queue += graph[person]  
				searched.append(person)  
	return False