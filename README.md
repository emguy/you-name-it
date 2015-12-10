younameit
=========

bash script for file renaming utilizing the editing power of VIM.

- requires the command-line editor VIM

##usage: 

    younameit [-hfqv] files_names ... 

        -h show this help text 
        
        -v show verion imformation 
        
        -f enable file overwrite
        
        -q quiet mode which suppresses all console messages
        

##example:

    younameit foo*.txt
    
    | 1  foo1.txt             | ~  1  bar1.txt           |
    | 2  foo1.txt             | ~  2  bar2.txt           |
    | 3  foo1.txt             | ~  3  bar3.txt           |
    | 4  foo1.txt             | ~  4  bar4.txt           |
    | 5  foo1.txt             | ~  5  bar5.txt           |
    | 6  foo1.txt             | ~  6  bar6.txt           |
    | 7                       | ~  7                     |
    | 8                       | ~  8                     |
    | ~                       | ~  ~                     |
    | ~                       | ~  ~                     |
    | ~                       | ~  ~                     |
    | ~                       | ~  ~                     |
    | ~                       | ~  ~                     |
    |younameit.before 1,1 all |younameit.after   1,1 all |
