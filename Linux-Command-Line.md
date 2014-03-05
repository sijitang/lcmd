Linux Command Line Collections 
======================

lcmd
-------

1. Serving HTTP on 0.0.0.0 port 8000
    ```bash
    python -m SimpleHTTPServer
    ```

2. save root file in vi when you forget typing sudo
    ```bash
    :w !sudo tee %
    ```

3. 在当前目录递归搜索单词”eat”,不匹配类似于”feature”或”eating”的字符串:
    ```bash
   $ ack -w eat
    ```

4. 搜索有特殊字符的字符串’$path=.’,所有的元字符（比如’$',’.')需要在字面上被匹配:
    ```bash
   ack -Q '$path=.' /etc
    ```

5. 除了dowloads目录，在所有目录搜索”about”单词
    ```bash
    $ ack about --ignore-dir=downloads
    ```

 6.只搜索包含’protected’单词的PHP文件，然后通过文件名把搜索结果整合在一起，打印每个文件对应的搜索结果:
    ```bash
    $ ack --php --group protected
    ```
 7.要换取ack支持的文件过滤类型，运行：
     ```bash
    $ ack --help-type
    ```



