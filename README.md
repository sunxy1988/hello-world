hello-world
===========

let's begin
```flow
    st=>start: Start|past:>http://www.baidu.com
    e=>end:  Ende|future:>http://www.baidu.com
    op1=>operation:  My Operation
    op2=>operation:  Stuff|current
    sub1=>subroutine:  My Subroutine|invalid
    cond=>condition:  Yes or No|approved:>http://www.google.com
    c2=>condition:  Good idea|rejected
    io=>inputoutput:  catch something...|future
    st->op1(right)->cond
    cond(yes, right)->c2
    cond(no)->sub1(left)->op1
    c2(yes)->io->e
    c2(no)->op2->e
```
