# Instructions append

## Board format

The board is represented as a null-terminated string, with a newline character at the end of each row.

An example would be `"X . . .\n . X O .\n  O . X O\n   . O . X\n    . . O .\n"`

## Registers

| Register | Usage        | Type    | Description                          |
| -------- | ------------ | ------- | ------------------------------------ |
| `$a0`    | input        | address | null-terminated input string         |
| `$v0`    | output       | byte    | 'O' or 'X', or '.' if nobody has won |
| `$t0-9`  | temporary    | any     | for temporary storage                |
