# Lesson 1
- [x] Learn the basic commands of VIM such as h j k l and move around.
It's very basic and easy.

# Lesson 2
- [x] Basic as well.
- [x] Type d[motion] to determine the motion you are looking for: $ means the end of line, e means the end of a word, w means an entire word
      Type dd to delete an entire line
      Type d$ to delete the line from the cursor
- [x] operator [number] motion lets you manipulate the text as you want.
      c 2 w deletes 2 words forward from the cursor and puts you in INSERT
      d 2 w deletes 2 words
        2 $ moves you two lines forward
	2 w moves you two words forward
- [x] Other commands: u to undo the one previous change you made
		      U to undo the changes you made to the entire line

# Lesson 3: Learn to place yourself!
- [x] dd deletes the entire line and puts it into a VIM register
      *p* will put the line **below** the cursor.
- [x] r command in NORMAL puts you to replace the character in the cursor position.
- [x] c [number] [motion] to manipulate the text!

# Lesson 4: Learn to locate yourself!
- [x] THE SEARCH COMMAND
	* In NORMAL type the / character and notice the bottom of screen will appear a / character as with the : command.
	* Type the word you are looking for and VIM will find it for you.
	* To search for the same phrase again, just type n
	* To search for the phrase in the opposite direction, type N
	* To search for a phrase in a backward direction, use ? instead of /
- [x] FIND MATCHIN PARATHESIS
	* Place the cursor on any {, [, ( and type the % character and the cursor will move to the matchin parathesis or bracket.
- [x] THE SUBSTITUTE COMMAND
	* In COMMAND, type s to enter substitute mode. :s/[old]/[new] where old is the word you are looking to replace and new it's the word you want to place.
	* Type   :#,#s/old/new/g    where #,# are the line numbers of the rangeof lines where the substitution is to be done.
	* Type   :%s/old/new/g      to change every occurrence in the whole file.
	* Type   :%s/old/new/gc     to find every occurrence in the whole file,with a prompt whether to substitute or not.

# Lesson 5: Learn to execute externally!
- [x] THE ! COMMAND
	* Type :! followed by an external command to execute that command! For example: !q to quit, !ls to list the current directory.
	NOTE: It's possible to execute any external command this way. Don't forget to hit ENTER afterwards.
- [x] WRITING FILES
	* Select a name that you want to save your file under.
	* Type :w [name] where [name] is the name you choose and you will have saved your file under that filename.
- [x] SELECT PART OF TEXT
	* Move the cursor to the line and press v to enter visual mode.
	* Now press : and you will also see :'<,'> at bottom which indicates that you successfully selected the target line and now repeat the process of the WRITING FILES to write these selected lines to the file

# Lesson 6: Manipulate texts and words
- [x] THE O COMMAND
	* Type o at any position in a line and this command will put you to a new line and into INSERT below the current line.
- [x] THE R MODE
	* Type R and VIM puts you to the REPLACE. From your cursor, now you can replace any characters.
 - [x] COPY AND PASTE
	* First, press v to enter VISUAL and manipulate the text with preferred manipulation we learned earlier. For example, v w to select a word, v 2 w to select two words and so on.
	* Then, press y to yank (copy) the chosen text.
	* Last, move the cursor to the preferred position and press p (paste)
- [x] SET OPTIONS
	* Type :set xxx sets the option xxx
		For example: 'ic': ignore case
