While learning and programming in Rust I realized that to understand the Rust language I need to understand the C. 
For some reasons I also in need of interpreter for Lisp like language in Rust.  
To learn the C, Lisp, and how to made interpreter for Lisp I made the tutorial:   
[Build Your Own Lisp](https://buildyourownlisp.com/contents)    
[Build Your Own Lisp; GitHub](https://github.com/orangeduck/BuildYourOwnLisp) 

The project / learning is in progress. 

```mpc.c``` and ```mpc.h``` files are downloaded from   
[orangeduck/mpc](https://github.com/orangeduck/mpc) the ```mpc``` parser library

Examples :   
```
$ cc -std=c99 -Wall parsing.c mpc.c -ledit -lm -o parsing
$ ./parsing
Lispy version 0.0.0.0.1
Press Ctrl+c to Exit
 
lispy> + 10 (* 5 5)
> 
  regex 
  operator|char:1:1 '+'
  expr|number|regex:1:3 '10'
  expr|> 
    char:1:6 '('
    operator|char:1:7 '*'
    expr|number|regex:1:9 '5'
    expr|number|regex:1:11 '5'
    char:1:12 ')'
  regex 
lispy> 
```

To be continued .. 


