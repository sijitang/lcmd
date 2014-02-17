Groovy Collections 
============

gryc
-------

1. groovy map sort with value, reverse sort
    ```python
    def map = [a:3, b:2, c:1]
    map = map.sort {it.value}
    assert map == 1
    ```

2. Turns out doing a reverse sort on a Map by values is almost as easy.
    ```python
    def map = [a:1, b:2, c:3]
    map = map.sort {a, b -> b.value <=> a.value}
    assert map == 1
    ```

