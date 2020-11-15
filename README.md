# vim-cheatsheet

https://vim.rtorr.com/

<b>You can always use esc to reset your ongoing command
Exit always in esc mode</b>
<b>:q</b> - quit<br>
<b>:wq</b> - save and quit<br>
<b>:q!</b> - don't save and quit<br>

<b>:w</b> - to save the file as we go

<b>l</b>  - right
<b>h</b>  - left
<b>k</b>  - up
<b>j</b>  = down

<b>you can put numbers before every command</b> 
<b>10k</b>  - move up 10 lines
<b>10l</b>  - move right 10 characters

<b>A number adds a multiplier</b> 

<b>}</b>  - move down in blocks
<b>{</b>  - move up in blocks

<b>w</b>  - move across words in right dir
<b>b</b>  - move across words in left dir
<b>W (Cap) / B (Cap)</b> - moves fast than w/b, ignores punctuations
<b>0</b>  - move to the beginning of the line
<b> ^ / 0w </b>  - move to the beginning of first word

<b>a</b>  - 1 step right + insert mode

<b>A</b>  - to the end of the line + insert mode
<b>I</b>  - to the beg of line + insert mode

<b>f(char)</b>  - find that character in line and cursor is on that char
<b>t(char)</b>  - find + cursor is 1 left to that char

<b>%</b>  called motion- can be used to move between opening and closing blocks , like from { to } directly

<b>d%</b>  - can be used to delete the whole block, covered by %, that is between a particular opening and closing of (,{,[

<b>d[--]</b>  - d can be used for delete with any type of command.

<b>cw</b>  - change word - deletes the word and puts cursor to that position for replacement and puts you into insert mode.

<b>dw</b>  - delete word - deletes the word

<b>ct(char)</b>  - we can change from cursor to particular char

<b>D (Cap)</b>  - deletes whole line to the right of cursor.
<b>C (Cap)</b>  - D(Cap) + insert mode

<b>*</b>  - used as ctrl f - to search instances of a word in a file.

<b>/ (word)</b>  - ctrl f - to search in a file
<b>n</b>  - to move to next instance in down dir
<b>N</b>  - to move to next instance in up dir

<b>* and /</b>   - both works

<b>t(char); / ;</b>  - to find a instance across a line , 

<b>x</b>  - deletes a char
<b>10x</b>  - 10 letters to the right

<b>r(char)</b>  - replace the char

<b>~</b>  - changes the case of a letter
<b>10~</b>  - will change case of 10 char to the right

<b>.</b>  (period operator) - does the last command performed, can be used to repeat the same command again and again 

<b>select + ></b>  - for indenting chunk of code

<b>gg</b>  - top of the file

<b>dd</b>  - delete the line
<b>10dd</b>  - delete 10 times
<b>dG</b>  - delete from current line to bottom line 
<b>u</b>  - undo 
<b>ctrl R</b>  - redo

<b>yy</b>  - can be used to copy a line
<b>p</b>  - paste below a particular line
<b>Capital P</b>  - paste above a particular line

<b>ctrl Cap V</b>  - puts you into visual mode
you can see your selection and do all the operations to that selection

<b>copy paste - </b> 
yy + p (for a line)
select + yy + p (in visual mode)
combination - y10j - copy 10 lines below and then use p.

<b>cut paste - </b> 
dd + P (for a line)
select + dd + P (in visual mode)
combination - d10j - delete 10 lines below and then use P.

<b>o</b>  - adds a \n down and puts you into insert mode.
<b>O</b>  - adds a \n above and puts into insert mode.

<b>zz</b>  - centers your file in your vim window.


Macros:
We can save some special set of commands to a particular key.
steps:
1. Press q
2. Press the key you wanna save the commands to (eg. w)
3. Set of commands you wanna record.
4. Again press q
5. you can access this macro using @(char). eg. (@w)
