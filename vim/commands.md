# Vim Commands

### Inserting Text

To insert text, press `i`. You will see the lower left hand of the screen change to `--INSERT--`. You can then begin inserting text. 

#### Appending Text
`a` inserts text **after** the cursor, while `i` inserts text **before** the cursor. 

#### Adding New Lines
`o` will add a line **below** the current, and position the cursor on the new line.
`O` will add a line **above** the current, and position the cursor on the new line.

#### Changing Text ####
`cw` will delete the next word, similar to `d` but will leave you insert mode. 
`C` will delete the line nstarting from your cursor position, similar to `D`, but again leave you in insert mode. 

### Moving Arround

You should use the `h`, `j`, `k`, `l` keys to move left, down, up, and right respectively.

> This will take some getting used to. Alternatively, you can use the arrow keys; however, this is much slower and hence not preffered. 

#### Word Movement
`w` will move the cursor **foward** one word. 
`b` will move the cursor **backward** one word. 

> from `:help word` : " 
> A **word** consists of a sequence of letters, digits, and underscores, or a sequence of other non-blank characters, separated with white spaces. 
> A **WORD** consists of a sequence of non-blank characters, separated with white space. An empty line is considered to be a  word. 

You can use counts to move faster. For example `5w` will move the cursor forward 5 words. Likewise, `5b` will move the cursor backwards 5 words. 

#### Begin / End of Line
Type `^` (or `0`) to move the cursor to the first non-blank character of the line. 
Type `$` to move the cursor to the last character of the line. 

#### Searching Along a Single Line ####
Use `fx` to move your cursor to the next occurence of **x** on the current line.
`3fx` will move your cursor to the third occurence of **x** on the current line.
Similarly, `Fx` will move your cursor to the previous occurence of **x** on the current line.

`tx` and `Tx` work exactly the same, except the cursor will stop one character prior to to **x**.

#### Move to Specific Line ####
Frequently, you will need to go to a specific line. This can be accomplished with `GN` command. For example `G156` will move the cursor to the beggining character of line 156. 

#### Where am I? ####
`Cntrl-G` displays a status line at the bottom of the screen indiciating your position in the file. 
`:set number` adds line numbers on the left.
`:set nonumber` removes those line numbers.
> These line numbers are informational only. They are not written to the file. 

#### Scrolling ####
To scroll half way down the screen, type `Cntrl-D`.


### Deleting 

To delete a character, move the cursor over it and press `x`.

To delete an entire line, type `dd` which will delete the line on which the cursor is positoned. 
Alternatively, `D` deletes the rest of the line starting from where your cursor is. 

To delete the next word, type `dw`. To delete the next **3** words type `d3w`. 

### Undo and Redo

To undo press `u` and to redo press `Cntrl-r`. 

### Getting Out

`ZZ` saves and quits. 
`:q!` quits without saving. 

`:help` will open the help window.
`:help x` will open help for the **x** topic.

