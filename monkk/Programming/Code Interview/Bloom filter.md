Bloom filters offer a solution ( if you have to check one item against millions of them)


Bloom filters are probabilistic data structures. They give you an answer that could be wrong but is probably сorrect. Instead of a hash, you can ask your bloom filter if you’ve  
crawled this URL before. A hash table would give you an accurate answer. A bloom filter will give you an answer that’s probably correct:
• False positives are possible. Google might say, “You’ve already crawled  
this site,” even though you haven’t.
• False negatives aren’t possible. If the bloom filter says, “You haven’t  
crawled this site,” then you definitely haven’t crawled this site.  

Bloom filters are great because they take up very little space. A hash  
table would have to store every URL crawled by Google, but a bloom  
filter doesn’t have to do that. They’re great when you don’t need an exact  
answer, as in all of these examples. It’s okay for bit.ly to say, “We think  
this site might be malicious, so be extra careful.”