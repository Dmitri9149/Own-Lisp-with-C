For some reasons I need interpreter for Lisp like language in Rust.  
(Some dealect of Scheme, to be more presise).       
As first step I study how to build 'own' Lisp with C with the tutorial   
[Build Your Own Lisp](https://buildyourownlisp.com/contents)    
[Build Your Own Lisp; GitHub](https://github.com/orangeduck/BuildYourOwnLisp) 

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

The work is in progress.


