# Personal HyperSnips snippet for VSCode

Require [HyperSnips](https://marketplace.visualstudio.com/items?itemName=draivin.hsnips) extension to be installed.

in Windows clone this repo to (don't clone to a subfolder):

```
%APPDATA%\Code\User\hsnips
```

# Created Snippets

## Javascript

| type  | trigger | description                                                      | Restriction |
| ----- | ------- | ---------------------------------------------------------------- | ----------- |
| Regex | func\d  | Creates function declaration block with `\d` number of arguments | Empty line  |
| Regex | afunc\d | Like `func\d` but using arrow function syntax                    | Empty line  |

## C++

| type       | trigger      | description                                                                     | Restriction |
| ---------- | ------------ | ------------------------------------------------------------------------------- | ----------- |
| Line Begin | cout         | creates cout print statement                                                    |             |
| Line Begin | cin          | creates cin extraction statement                                                |             |
| Line Begin | inc< \| inc" | creates include statement with target text surround by either bracket or quotes |             |
| Regex      | func\d       | creates function declaration with `\d` number of arguments                      | Empty line  |
| Regex      | funcc\d      | creates function declaration with doc comments and `\d` number of arguments     | Empty line  |
| Regex      | hfuncc\d     | creates function prototype with doc comments and `\d` number of arguments       | Empty line  |
