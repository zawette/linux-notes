# vim cheatsheet 
> ps : \<cr> synbolizes a carriage return (enter)
## basic movements
+ hjkl left down top right
+ gg first line of the file
+ G last line of the file
+ 0 beginning of the line
+ $ end of the line
+ w next word ( W by whitespace)
+ b previous word (B by whitespace)
+ e end of word (E by whitespace)
+ % move to the next bracket or brace on the current line 
+ CTRL+u move up by half a page
+ CTRL+d move down by half a page
+ CTRL+b move up by a page
+ CTRL+f move down by a page
## searching
+ / search for word, cycle through results with n and N 
+ \* search for occurences of the word where cursor is pointing with * 
+ clear search highlights => :noh \<cr> 
+ fc move cursor to next occurence of c on the current line (F for previous occurence)
+ tc move cursor till next occurence of c on the current line (T for previous occurence)
## insertion
+ i inserts where the cursor is ( I inserts at the beginning of the line)
+ a inserts next to the cursor (A inserts at the end of the line)
+ o inserts below the the current line (O insert above the current line)
+ gi inserts in the last insert position
+ r replace char
+ cw change word
+ cc change whole line
+ C change from cursor to the end of the line
## deletion
+ x delete char (X backward), can achieve same results with dh and dl 
+ dh dj dk dl deletes in specified direction
+ dd delete whole line
+ D deletes from cursor to the end of the line
## yanking
+ yy yank line
+ yw yank word
+ ynw yank n word
+ y0 yank from cursor to the beginning of the line
+ y$ yank from cursor to the end of line
+ J join current line with the next one
## Visual mode
+ v highlight chars (V highlight lines)
+ CTRL+v highlight blockwise 
+ << shift left (>> shift right)
