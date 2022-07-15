## Outline
- redirection
- pipe
- difference between redirection and pipe


## Quick Overview
*refers[1], [2]* <br/>
**Pipe** is used to pass output to another program or utility.
**Redirect** is used to pass output to either a file or stream.

A **pipe** connects the stdout of one process to the stdin of another, 
whereas **redirection** redirects from/to a file (> from stdout to a file, < from a file to stdin)



Example: `thing1 > thing2` vs `thing1 | thing2`

`thing1 > thing2`
Your shell will run the program named `thing1`
Everything that `thing1` outputs will be placed in a file called `thing2`. (Note - if `thing2` exists, it will be overwritten)
If you want to pass the output from program `thing1` to a program called `thing2`, you could do the following:

`thing1 > temp_file && thing2 < temp_file`

which would
- run program named `thing1`
- save the output into a file named `temp_file`
- run program named `thing2`, pretending that the person at the keyboard typed the contents of `temp_file` as the input.<br/>
However, that's clunky, so they made pipes as a simpler way to do that. `thing1 | thing2` does the same thing as `thing1 > temp_file && thing2 < temp_file`


## Pipe usage
*refers [3]*

## Redirect usage
*refers [4]*

## Diff between pipe and redirection
*refers [3]*

## References
[1] https://askubuntu.com/questions/172982/what-is-the-difference-between-redirection-and-pipe <br/>
[2] https://superuser.com/questions/277324/pipes-vs-redirects#:~:text=The%20difference%20lies%20in%20how,from%20a%20file%20to%20stdin)<br/>
[3] https://www.cnblogs.com/chengmo/archive/2010/10/21/1856577.html <br/>
