1. The line `query_set=Product.objects.all()` retrieves all instances of the `Product` model using the `all()` method on the `objects` manager. 
    
2. `objects` manager has methods like `all()`, `get()`, and more. In Django, the manager is responsible for handling queries to the database table.
    
3. The next commented section  iterating through each product in the `query_set` and printing its details. 
    
4. The following line `print(query_set[0].title)` prints the `title` attribute of the first item in the `query_set`. This will trigger a database query to retrieve the first item's title. The comment below explains that performing any action like indexing will create a query to fetch the data.
    
5. The comment explains that every action performed on the `query_set` will result in a query being executed. Django uses a mechanism called "lazy evaluation," which means the query is executed only when the data is required.
    
6. The comment provides two examples:
    
    - Example one: If you loop through the entire `query_set`, a separate query will be executed for each iteration.
    - Example two: If you access only a single item with `query_set[0]`, Django will create a query with a `LIMIT 1` clause to fetch just one item from the database.
7. The comment further mentions that some methods, like `count()`, return results immediately instead of returning a queryset. These methods don't require the query to be executed since they don't need the actual data, just some aggregate information.


```python
def say_hello(request):
    # each model will have something call objects
    # on objects all() get and some more methods
    # doing all will return queryset
    query_set=Product.objects.all()
    # for product in query_set:
    #     print(product)
    # if we will perform any action then only it will create a query will be create
    print(query_set[0].title)
    # why because in evalutuate everything that we are doing then create our query
    # example one it will create query for every data
    # example two it will create query for data with limit 1
    # there are some method which return result imediately like count() instead of query_set
 
    return render(request, 'hello.html', {'name': 'Mosh'})
```


# To see query response 

In django developement tool Click on the "SQL" panel to see the list of executed SQL queries, their execution time, and other related information. You can expand each query to see more details, including the actual SQL statement and the parameters used in the query.