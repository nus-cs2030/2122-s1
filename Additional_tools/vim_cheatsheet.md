# Vim Cheat sheet

____

This markdown file mainly aims to provide some useful commands suggested. 

Do feel free to update this list with commands that you think is useful. 



## File Navigation and UI Command

- `:e <filename>` Exit the current open file and open the new file specified.
- `:split` Split the current window horizontally into 2
- `:vert split`, `:vsp` Split the current window vertically into 2
- `:vert term` vertically split a terminal session.
- `^W/<ctrl+w>` followed by `<arrow keys/hjkl>`  to navigated between opened split screen windows
- `:!<shell command>` Immediately execute terminal commands in vim



## Cursor Navigation and Quick Editing Command

- `i`  Enter insert mode at with the cursor <u>before the current character.</u>

- `I` Enter insert mode at with the cursor <u>at the first non-whitespace character of the line</u> 

- `a`  Enter insert mode at with the cursor <u>after the current character.</u>

- `A` Enter insert mode at with the cursor <u>at the end of the line</u>

- `$` cursor to last character of the line

- `^` cursor to first  non-whitespace character of the line

- `gg` cursor to start of file

- `G` cursor to end of file

- `gg=G` auto indent entire file

- `dd` or `D` cut/delete the line your cursor is on

- `d` cut/delete marked text

- `<start line>,<end line>d` cut/delete text between line number specified

- `y` copy marked text

- `<start line>,<end line>d` copy/yank text between line number specified

- `Y` ,`yy` copy/yank the entire line your cursor is on

- `w` jump forward to start of a word

- `b` jump back to start of a word

- `p` paste in text (stored in vim, diff from ctrl+v)

- `x` delete key when not in insert mode

- `X` backspace key when not in insert mode

  



## Others

- `ZZ` , `:wq` Save and quit
- `:s/<regex pattern>/<replaced text>/<regex flags>` search and replace using regular expressions on the current line your cursor is on
- `:%s/<regex pattern>/<replaced text>/<regex flags>` search and replace using regular expressions on the whole file
- `:<startline>,<endline>s/<regex pattern>/<replaced text>/<regex flags>` search and replace using regular expressions on the text between the start line and end line.

Note if you confused with what regex search and replace, you can just think of it as /search_string/replace_string/g to replace all instance of search_string with replace_string in the range specified but take note some special characters like `.` will cause some issues if you use them like normal search and replace.

