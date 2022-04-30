## Pagination   
The following are the project objectives:  
* How to paginate a dataset with simple page and page_size parameters
* How to paginate a dataset with hypermedia metadata   
* How to paginate in a deletion-resilient manner   

### Resources   
* [REST API Design: Pagination](https://www.moesif.com/blog/technical/api-design/REST-API-Design-Filtering-Sorting-and-Pagination/#pagination)
* [HATEOAS](https://en.wikipedia.org/wiki/HATEOAS)  

## Tasks
* **Task 0: Simple helper function**   
Write a function named `index_range` that takes two integer arguments `page` and `page_size.`    
The function should return a tuple of size two containing a start index and an end index corresponding to the range of indexes to return in a list for those particular pagination parameters.    
Page numbers are 1-indexed, i.e. the first page is page 1.   

