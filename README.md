# Shell
A Basic Prompt Shell
Created by Sam Mergendahl (github.com/smergendahl) and Colin Samplawski (github.com/colinski)

We simply wrote a program that read in input from either file or an input file
(using dup() and dup2() to redirect stdout). Then each line was parsed and saved 
into history which was a circular arry. Then we checked to see if the input line 
was a history or exit command. If it was neither, the line was passed to execvp
,after first forking the running process. Incorrect commands were caught there.
