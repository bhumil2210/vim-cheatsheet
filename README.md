# vim-cheatsheet

https://vim.rtorr.com/

You can always use esc to reset your ongoing command
Exit always in esc mode
:q - quit
:wq - save and quit
:q! - don't save and quit

:w - to save the file as we go

l - right
h - left
k - up
j = down

you can put numbers before every command
10k - move up 10 lines
10l - move right 10 characters

A number adds a multiplier

} - move down in blocks
{ - move up in blocks

w - move across words in right dir
b - move across words in left dir
W (Cap) / B (Cap)- moves fast than w/b, ignores punctuations
0 - move to the beginning of the line
^ / 0w - move to the beginning of first word

a - 1 step right + insert mode

A - to the end of the line + insert mode
I - to the beg of line + insert mode

f(char) - find that character in line and cursor is on that char
t(char) - find + cursor is 1 left to that char

% called motion- can be used to move between opening and closing blocks , like from { to } directly

d% - can be used to delete the whole block, covered by %, that is between a particular opening and closing of (,{,[

d[--] - d can be used for delete with any type of command.

cw - change word - deletes the word and puts cursor to that position for replacement and puts you into insert mode.

dw - delete word - deletes the word

ct(char) - we can change from cursor to particular char

D (Cap) - deletes whole line to the right of cursor.
C (Cap) - D(Cap) + insert mode

* - used as ctrl f - to search instances of a word in a file.

/ (word) - ctrl f - to search in a file
n - to move to next instance in down dir
N - to move to next instance in up dir

* and /  - both works

t(char); / ; - to find a instance across a line , 

x - deletes a char
10x - 10 letters to the right

r(char) - replace the char

~ - changes the case of a letter
10~ - will change case of 10 char to the right

. (period operator) - does the last command performed, can be used to repeat the same command again and again 

select + > - for indenting chunk of code

gg - top of the file


dd - delete the line
10dd - delete 10 times
dG - delete from current line to bottom line 
u - undo 
ctrl R - redo

yy - can be used to copy a line
p - paste below a particular line
Capital P - paste above a particular line

ctrl Cap V - puts you into visual mode
you can see your selection and do all the operations to that selection

copy paste - 
yy + p (for a line)
select + yy + p (in visual mode)
combination - y10j - copy 10 lines below and then use p.

cut paste - 
dd + P (for a line)
select + dd + P (in visual mode)
combination - d10j - delete 10 lines below and then use P.

o - adds a \n down and puts you into insert mode.
O - adds a \n above and puts into insert mode.

zz - centers your file in your vim window.


Macros:
We can save some special set of commands to a particular key.
steps:
1. Press q
2. Press the key you wanna save the commands to (eg. w)
3. Set of commands you wanna record.
4. Again press q
5. you can access this macro using @(char). eg. (@w)
