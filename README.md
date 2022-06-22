# Drawing-Robot

Developing a _GUI_ that converts a source program that contains _basic commands_ and controls the position of a _virtual pen_ on the computer screen to the corresponding image

WHAT PURPOSES?

The designed VM (Virtual Machine) reads any selected .txt file and draws lines according to the commands in it. (An example file: [example.txt](https://github.com/elifkapln/Drawing-Robot/files/8884803/example_txt.txt) )

HOW TO USE?

- After the program is run, the **Choose File** button is clicked to select the .txt file from which the commands will be read.
- Commands contained in the selected file are displayed on _the blue panel.
- If there is no **'syntax'** error in the commands, the drawing is made to _the white panel.
- If an error is detected in the commands, the error message is displayed on _the green panel.

HOW DOES IT WORK?

The Line Drawer VM performs **'lexical analysis'** of the commands contained in the file it reads. It performs the **'parsing'** operation according to the **'syntax'** rules previously determined by the grammars. 
If an error is detected at this point, the error message is displayed on the green panel. If the commands taken from the file are correct, the drawing is made.

WHAT IS REQUIRED TO RUN?

This program is in _VS Code_ platform and it has been programmed with Turtle, Tkinter and PLY (LEX/YACC) of _Python_ language. The **lex.py** and **yacc.py** files are necessary and sufficient to run the program.
