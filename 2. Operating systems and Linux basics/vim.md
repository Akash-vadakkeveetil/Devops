<h1 align="center">Working with VIM Editior</h1>
<hr>

Vim is a command line text editor which is widely used all over the world, let's dive into the commands which we need to navigate through the VIM editor 

👉 **Opening/Creating Files:**

- Open or create a new file: `vim <file name>`

👉 **Exiting Vim:**

- Exit Vim: `:q`

👉 **Command Mode:**

- Enter command mode: `:`

👉 **Syntax and Line Numbers:**

- Turn on syntax highlighting: `:syntax on`
- Set line numbers: `:set nu`

👉 **Navigation:**

- Left: `h`
- Down: `j`
- Up: `k`
- Right: `l`
- Move by word: `w`
- Move by previous word: `b`
- Beginning of the line: `0`
- End of the line: `$`
- Move to the beginning of the word: `^`
- First line: `gg`
- End of the document: `G`
- Move left and right sentence by sentence: `[ ]`
- Go to the starting of a specific line: `<line number> + gg`

👉 **Insert and Save:**

- Enter insert mode: `i`
- Save: `:w`
- Save and quit: `:wq`

👉 **Undo and Redo:**

- Undo: `u`
- Redo: `ctrl + r`

👉 **Appending and Inserting:**

- Append after the current character: `a`
- Insert after the current line: `o`
- Insert before current line: `shift + o`
- Append at the end of the line: `shift + a`

👉 **Deletion and Cutting:**

- Delete the word: `dw`
- Delete the current line: `dd`
- Delete a specific line: `<line number>dd`
- Delete everything: `dG`
- Cut the line: `dd`

👉 **Paste and Search:** - Paste the line after using `dd`: `p` - Delete before the word: `db` - Search for a word: `/<word>` - Next search result: `n` - Previous search result: `N`

👉 **Find and Replace:** - Find and replace: `:%s/<word to be replaced>/word with to be replaced`