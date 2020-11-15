# vim-cheatsheet

https://vim.rtorr.com/

<b>You can always use esc to reset your ongoing command
Exit always in esc mode</b>
<b>:q</b> - quit<br>
<b>:wq</b> - save and quit<br>
<b>:q!</b> - don't save and quit

<b>:w</b> - to save the file as we go

<b>l</b>  - right<br>
<b>h</b>  - left<br>
<b>k</b>  - up<br>
<b>j</b>  = down<br>

<b>you can put numbers before every command</b><br>
<b>10k</b>  - move up 10 lines<br>
<b>10l</b>  - move right 10 characters<br>

<b>A number adds a multiplier</b> 

<b>}</b>  - move down in blocks<br>
<b>{</b>  - move up in blocks<br>

<b>w</b>  - move across words in right dir<br>
<b>b</b>  - move across words in left dir<br>
<b>W (Cap) / B (Cap)</b> - moves fast than w/b, ignores punctuations<br>
<b>0</b>  - move to the beginning of the line<br>
<b> ^ / 0w </b>  - move to the beginning of first word<br>

<b>a</b>  - 1 step right + insert mode<br>

<b>A</b>  - to the end of the line + insert mode<br>
<b>I</b>  - to the beg of line + insert mode<br>

<b>f(char)</b>  - find that character in line and cursor is on that char<br>
<b>t(char)</b>  - find + cursor is 1 left to that char<br>

<b>%</b>  called motion- can be used to move between opening and closing blocks , like from { to } directly

<b>d%</b>  - can be used to delete the whole block, covered by %, that is between a particular opening and closing of (,{,[

<b>d[--]</b>  - d can be used for delete with any type of command.

<b>cw</b>  - change word - deletes the word and puts cursor to that position for replacement and puts you into insert mode.

<b>dw</b>  - delete word - deletes the word

<b>ct(char)</b>  - we can change from cursor to particular char

<b>D (Cap)</b>  - deletes whole line to the right of cursor.<br>
<b>C (Cap)</b>  - D(Cap) + insert mode

<b>*</b>  - used as ctrl f - to search instances of a word in a file.

<b>/ (word)</b>  - ctrl f - to search in a file<br>
<b>n</b>  - to move to next instance in down dir<br>
<b>N</b>  - to move to next instance in up dir

<b>* and /</b>   - both works

<b>t(char); / ;</b>  - to find a instance across a line , 

<b>x</b>  - deletes a char<br>
<b>10x</b>  - 10 letters to the right

<b>r(char)</b>  - replace the char

<b>~</b>  - changes the case of a letter<br>
<b>10~</b>  - will change case of 10 char to the right

<b>.</b>  (period operator) - does the last command performed, can be used to repeat the same command again and again 

<b>select + ></b>  - for indenting chunk of code

<b>gg</b>  - top of the file

<b>dd</b>  - delete the line<br>
<b>10dd</b>  - delete 10 times<br>
<b>dG</b>  - delete from current line to bottom line <br>
<b>u</b>  - undo <br>
<b>ctrl R</b>  - redo

<b>yy</b>  - can be used to copy a line<br>
<b>p</b>  - paste below a particular line<br>
<b>Capital P</b>  - paste above a particular line

<b>ctrl Cap V</b>  - puts you into visual mode<br>
you can see your selection and do all the operations to that selection

<b>copy paste - </b> <br>
yy + p (for a line)<br>
select + yy + p (in visual mode)<br>
combination - y10j - copy 10 lines below and then use p.

<b>cut paste - </b> <br>
dd + P (for a line)<br>
select + dd + P (in visual mode)<br>
combination - d10j - delete 10 lines below and then use P.

<b>o</b>  - adds a \n down and puts you into insert mode.<br>
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
