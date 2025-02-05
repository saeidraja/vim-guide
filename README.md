# vim-guide

### Find and Replace with Control Over Each Occurrence

The equivalent of `Ctrl+H` in VSCode (Find and Replace with control over each occurrence) can be achieved in Vim using the following command:

```vim
:%s/=/:/gc
```

#### Explanation:
- `:%` → Apply the command to the entire file.
- `s` → Substitution command.
- `/=` → The pattern to search for (in this case, `=`).
- `:` → The text to replace it with.
- `g` → Replace all occurrences in each line (not just the first).
- `c` → Prompt for confirmation before replacing each match.

### shift the selected lines (shift+v) one space to the left without affecting the current indentation structure

```vim
:s/^ //
```
#### Explanation:
- if you use two spaces after ^ , the lines shifted two spaces to the left
