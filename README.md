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

