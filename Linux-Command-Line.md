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
   $ ack -Q '$path=.' /etc
    ```

5. 除了dowloads目录，在所有目录搜索”about”单词
    ```bash
    $ ack about --ignore-dir=downloads
    ```

6. 只搜索包含’protected’单词的PHP文件，然后通过文件名把搜索结果整合在一起，打印每个文件对应的搜索结果:
    ```bash
    $ ack --php --group protected
    ```

7. 要换取ack支持的文件过滤类型，运行：
     ```bash
    $ ack --help-type
    ```

8. use less command to view log
     ```bash
    $ less -Rinf gs-admin.log
    ```

9. cd switch between latest directory
     ```bash
    $ cd -
    ```

10. use less command to view log
     ```bash
    $ less -Rinf gs-admin.log
    ```

11. list human readable files
     ```bash
    $ ls -lha 
    ```

12. find 
     ```bash
    $ find /var -name basic.ics 
    $ find /var -user sijitang 
    ```

13. locate 
     ```bash
    $ locate -i basic.ics 
    ```

14. history 
     ```bash
    $ history|grep ps
    ```

15. ctrl+L  = clear

16. ctrl+D = exit

17. unzip chinese language file 
     ```bash
    $ unzip -O cp936 luo.zip
    ```

18. List open network ports and sockets
     ```bash
    $ lsof -i
    ```

19. Periodically execute the specified command
     ```bash
    $ watch -n 10 who
    ```

20. screen
     ```bash
    $ screen
    create new screen: ctrl+A - C
    switch screen: ctrl+A - N
    detach screen: ctrl+A - D
    retach screen: screen -r xxx
    ```

21. find bios(   Linux-Dell-Bios-Info)
```bash
sudo dmidecode -s bios-version
sudo dmidecode -s bios-release-date
 ```