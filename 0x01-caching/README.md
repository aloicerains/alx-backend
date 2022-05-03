## Caching
The following are the project objectives:  
* What a caching system is
* What FIFO means
* What LIFO means
* What LRU means
* What MRU means
* What LFU means
* What the purpose of caching system
* What limits a caching system have

## Resources
The following resources are provided:
* [Cache replacement policies -FIFO](https://en.wikipedia.org/wiki/Cache_replacement_policies#First_In_First_Out_%28FIFO%29)   
* [Cache replacement policies-LIFO](https://en.wikipedia.org/wiki/Cache_replacement_policies#Last_In_First_Out_%28LIFO%29)  
* [Cache replacement policies-LRU](https://en.wikipedia.org/wiki/Cache_replacement_policies#Least_Recently_Used_%28LRU%29)
* [Cache replacement policies-MRU](https://en.wikipedia.org/wiki/Cache_replacement_policies#Least_Recently_Used_%28LRU%29)
* [Cache replacement policies-LFU](https://en.wikipedia.org/wiki/Cache_replacement_policies#Least_Recently_Used_%28LRU%29)
* [LRU caching](https://realpython.com/lru-cache-python/)

## Tasks
* **Task 0:**
Create a class `BasicCache` that inherits from `BaseCaching` and is a caching system:    
* You must use `self.cache_data` - dictionary from the parent class `BaseCaching`     
* This caching system doesn’t have limit
* `def put(self, key, item):`
* Must assign to the dictionary `self.cache_data` the `item` value for the `key` key.    
* If `key` or `item` is `None`, this method should not do anything.    
`def get(self, key):`   
* Must return the value in self.cache_data linked to key.
* If `key` is `None` or if the key doesn’t exist in `self.cache_data`, return `None`
* **Task 1:**   
Create a class `FIFOCache` that inherits from `BaseCaching` and is a caching system:    
You must use `self.cache_data` - dictionary from the parent class BaseCaching  
You can overload `def __init__(self):` but don’t forget to call the parent init: `super().__init__()`     
`def put(self, key, item):`    
* Must assign to the dictionary `self.cache_data` the `item` value for the key `key`.     
* If `key` or `items` is `None`, this method should not do anything.   
* If the number of items in `self.cache_data` is higher that `BaseCaching.MAX_ITEMS:`   
* you must discard the first item put in cache (FIFO algorithm)   
* you must print `DISCARD:` with the `key` discarded and following by a new line   
* `def get(self, key):`
* Must return the value in `self.cache_data` linked to `key`.
* If `key` is `None` or if the `key` doesn’t exist in `self.cache_data`, return `None`    
* **Task 2:**

