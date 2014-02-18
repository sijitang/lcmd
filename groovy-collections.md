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

3. Dae, TimeCategory
    ```python
    def today = new Date()
    today = today.clearTime()
    today = today.minus(2) // minus 2 days
    ```
    ```python
    import groovy.time.TimeCategory

    use(TimeCategory) {
            today = today + 23.hours + 59.minutes + 59.seconds
    }
    ```

4. Counting the Items in a List
    ```python
    def list = [0, 1, 2, 1, 1, 3, 2, 0, 1]
    list.size()
    list.count(0)
    list.count(1)
    list.count(2)
    list.count(3)
    ```
