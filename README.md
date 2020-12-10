# Website Test

## Set website url

Create a file `./url.txt` and put your URL inside the file. File must be in same folder.

## Set screen resolution

Create a file `./screen.txt` and put your screen size inside that file. Screen size should be in Width, Height

Ex:
```
1366,786
1024,768
360,640
786,1024
960,600
```

## Executing Test

Create a file `./task.txt` and put your execution sequence inside that file.

The execution code should be written as: `[Command]: [Statment]` 

Example:
```
c: //button[@id="my_btn"]
h: //div[@id="MC8mtf"]
w: 1
s: 200
t: //input[@id="name"] Hello world
t: //input[@id="email"] CONTROL a
t: //input[@id="search"] RETURN
j: console.log("Pass")
w: 1
```

### Some valid execution code is 
 - C : for click
 - H : Mouse hover
 - T : Type a text
 - S : Scroll down or up
 - J : Execute JavaScript
 - W : Wait or sleep

### Clicking at any element

Syntax: `C: xpath`

xpath : xpath of element where to click

### Mouse hover at any element

Syntax: `H: xpath`

xpath : xpath of element where to click

### Type a text

Syntax: 
 - `T: xpath <your_text>`
 - `T: xpath <special_key> <with_key>`
 - `T: xpath <special_key> <with_key>`

Example:
```
t: //input[@type="text"] Here is my text
t: //input[@type="text"] CONTROL a
t: //input[@type="text"] RETURN
```

`Line 1` is used to type plain text
`Line 2` is used for press [Ctrl]+A
`line 3` is used for hit enter key



### Scroll

Syntax: `S: <pixels>`

pixels : (integer) Absulute depth to be scrolled or zero(0) to scroll to bottom.

Ex:
```
S: 400
s: -200
s: 0
```

### Execute JavaScript

Syntax: `C: javascript`

javascript : inline JavaScript code you want to run


### Wait for a while

Syntax: `W: second`

second : Number of second you want to wait

### Special Keys
- ADD
- ALT
- ARROW_DOWN
- ARROW_LEFT
- ARROW_RIGHT
- ARROW_UP
- BACKSPACE
- BACK_SPACE
- CANCEL
- CLEAR
- COMMAND
- CONTROL
- DECIMAL
- DELETE
- DIVIDE
- DOWN
- END
- ENTER
- EQUALS
- ESCAPE
- F1
- F10
- F11
- F12
- F2
- F3
- F4
- F5
- F6
- F7
- F8
- F9
- HELP
- HOME
- INSERT
- LEFT
- LEFT_ALT
- LEFT_CONTROL
- LEFT_SHIFT
- META
- MULTIPLY
- NULL
- NUMPAD0
- NUMPAD1
- NUMPAD2
- NUMPAD3
- NUMPAD4
- NUMPAD5
- NUMPAD6
- NUMPAD7
- NUMPAD8
- NUMPAD9
- PAGE_DOWN
- PAGE_UP
- PAUSE
- RETURN
- RIGHT
- SEMICOLON
- SEPARATOR
- SHIFT
- SPACE
- SUBTRACT
- TAB
- UP
