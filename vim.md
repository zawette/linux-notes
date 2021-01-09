# vim cheatsheet 
> ps : \<cr> synbolizes a carriage return (enter)
## basic movements
+ hjkl left down top right
+ gg first line of the file
+ G last line of the file
+ :n or nG to jump to line n
+ 0 beginning of the line
+ $ end of the line
+ w next word ( W by whitespace)
+ b previous word (B by whitespace)
+ e end of word (E by whitespace)
+ % move to the next bracket or brace on the current line 
+ { and } to hop back and forth btw empty lines
+ CTRL+u move up by half a page
+ CTRL+d move down by half a page
+ CTRL+b move up by a page
+ CTRL+f move down by a page
+ mc marks a line in a file (capital char to mark globaly) , 'c to go to that mark
## searching
+ / search for word, cycle through results with n and N 
+ \* search for occurences of the word where cursor is pointing with * 
+ clear search highlights => :noh \<cr> 
+ fc move cursor to next occurence of c on the current line (F for previous occurence) , cycle through occurences with , and ;
+ tc move cursor till next occurence of c on the current line (T for previous occurence) cycle through occurences with , and ;
## insertion
+ i inserts where the cursor is ( I inserts at the beginning of the line)
+ a inserts next to the cursor (A inserts at the end of the line)
+ o inserts below the the current line (O insert above the current line)
+ gi inserts in the last insert position
+ ni inserts n times
+ r replace char
+ cw change word
+ ciw change word (if in the middle)
+ ci{ change inside { also works with ([
+ cc change whole line
+ C change from cursor to the end of the line
+ ctc change till c (cfc also exists)
## deletion
+ x delete char (X backward), can achieve same results with dh and dl 
+ s delete char and enter insert mode
+ dh dj dk dl deletes in specified direction
+ dd delete whole line
+ D deletes from cursor to the end of the line
+ ndd or dnd delete n lines
+ dtc deletes till c , example: dt) deletes everything till closing parenthesis
+ dfc deletes all the way up to c including c
+ dw delete word
+ diw delete word (if in the middle)
+ di{ delete inside { , also works with ([
+ dip deletes contiguous block of code
+ da{ , daw , dap also exists, for instance, da{ would delete everything inside { and the brackets themselves
## yanking
+ yy yank line
+ yw yank word
+ yiw yank the word (if in the middle of the word)
+ yi{ yank inside { also works with ([ 
+ ynw yank n word
+ ytc yank till c (yfc also exists)
+ P paste before, p paste after
+ y0 yank from cursor to the beginning of the line
+ y$ yank from cursor to the end of line
+ J join current line with the next one
## Visual mode
+ v highlight chars (V highlight lines)
+ CTRL+v highlight blockwise 
+ vfc highlight all the way up to c including c (vtc highlight till c) 
+ vw highlight word
+ viw highlight word (if in the middle) 
+ vi{ highlight inside { also works with ( [ 
+ << shift left (>> shift right)
## splits
+ CTRL+w v opens vertical split
+ CTRL+w s opens horizontal split 
+ :split file  open file in horizontal split 
+ :vs file  open file in vertical split
+ :resize n  where n is nb of rows 
+ :vertical resize n  where n is nb of columns 
+ CTRL+w = equally spread splits
+ CTRL+w CTRL+w switch btw windows
+ CTRL+w UP     Move to the top 
+ CTRL+w DOWN   Move to the bottom 
+ CTRL+w LEFT   Move to the left 
+ CTRL+w RIGHT  Move to the right 
## tabs
+ :tabe file - opens file in a new tab
+ :tabe new - opens new empty tab
+ :tabc - close tab
+ :tabs - list tabs
+ :tabn and tabp - next and previous tab
+ :tabfirst - go to first tab
+ :tablast - go to last tab
+ gt go to next tab (gT previous tab)
## other stuffs
+ insert the same characters across multiple lines https://stackoverflow.com/questions/9549729/vim-insert-the-same-characters-across-multiple-lines
