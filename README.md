---
title: ISPF Editor Cheatsheet
---

The following commands can be issued in the line number column (just type over the line numbers).

## Commands

|  command | explanation                                                  |
| -------: | ------------------------------------------------------------ |
|      `i` | insert line                                                  |
|      `o` | overwrite line (from previously copied or moved line)        |
|      `a` | insert above (from previously copied or moved line)          |
|      `b` | insert below (from previously copied or moved line)          |
|      `c` | copy line                                                    |
|      `r` | repeat line                                                  |
|      `m` | move line                                                    |
|      `x` | exclude/hide line (hide line for the current editor session) |
|      `f` | unhide line                                                  |
|      `(` | shift line to left                                           |
|      `)` | shift line to right                                          |
|      `<` | shift line to left, but respecting the mask                  |
|      `>` | shift line to right, but respecting the mask                 |
|     `uc` | make uppercase, block command is `ucc`                       |
|     `lc` | make lowercase, block command is `lcc`                       |
|   `mask` | set mask (using < character as start and > as end point)     |
| `bounds` | display current bounds                                       |

## Modifiers

- **repeat**: `COMMAND#`, for example `i10` to insert 10 lines
- **before/after**: adding `a` or `b` to apply the command before or after the current line
- **block alteration**: `COMMANDCOMMAND` to start the block and `COMMANDCOMMAND` to end the block, for example `cc` to start the block to copy and `cc` to end it.
