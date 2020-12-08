# Personal HyperSnips snippet for VSCode

# Requirements

1. Require [HyperSnips](https://marketplace.visualstudio.com/items?itemName=draivin.hsnips) extension to be installed.
2. You know what Regex is

# Snippet Types

| Type       | Description                                                                                                           |
| ---------- | --------------------------------------------------------------------------------------------------------------------- |
| Regex      | Auto-expand when you type according to regex and restriction is met. They will not appear on autocomplete selections. |
| Line Begin | Appears on autocomplete if before snippet location is empty (only whitespaces)                                        |
| Basic      | Appears on autocomplete everywhere                                                                                    |

# Install Instruction

Install [HyperSnips](https://marketplace.visualstudio.com/items?itemName=draivin.hsnips).

Then clone this repo.

in Windows clone this repo to (don't clone to a subfolder):

```
%APPDATA%\Code\User\hsnips
```

In Linux, clone this repo to (don't clone to a subfoler):

```url
$HOME/.config/Code/User/hsnips
```

# Demo

### Declaring by typing `class2` on VSCode

![2 variables class declaration](https://i.imgur.com/KB8cckh.gif)

### Declaring by typing `class4` on VSCode

![4 Variables class declaration](https://i.imgur.com/wsNfRhj.gif)

# Created Snippets

## Javascript

| type       | trigger   | description                                                                                                        | Restriction |
| ---------- | --------- | ------------------------------------------------------------------------------------------------------------------ | :---------: |
| Regex      | func\d    | Creates function declaration block with `\d` number of arguments                                                   | Empty line  |
| Regex      | funcc\d   | Creates function with docs with `\d` number of arguments                                                           | Empty line  |
| Regex      | afunc\d   | Like `func\d` but using arrow function syntax                                                                      | Empty line  |
| Regex      | afuncc\d  | Creates arrow function with docs with `\d` number of arguments                                                     | Empty line  |
| Regex      | edfuncc\d | Creates module export function with docs with `\d` number of arguments                                             | Empty line  |
| Line Begin | mde       | Creates `modules.exports` output statement                                                                         |             |
| Line Begin | req       | Creates `require` statement, while automatically convert dashes and underscores to camelcase on variable creation. |             |
| Line Begin | reqcc     | Creates `require` statement, enforcing camelcase on variable creation                                              |             |
| Line Begin | reqpc     | Creates `require` statement, enforcing pascal case on variable creation                                            |             |
| Line Begin | reqdes    | Creates `require` statement in destructure manner                                                                  |             |
| Regex      | class\d   | Class declaration with `\d` number of arguments                                                                    | Empty line  |

## C++

| type       | trigger      | description                                                                     | Restriction |
| ---------- | ------------ | ------------------------------------------------------------------------------- | :---------: |
| Line Begin | cout         | creates cout print statement                                                    |             |
| Line Begin | cin          | creates cin extraction statement                                                |             |
| Line Begin | inc< \| inc" | creates include statement with target text surround by either bracket or quotes |             |
| Regex      | func\d       | creates function declaration with `\d` number of arguments                      | Empty line  |
| Regex      | funcc\d      | creates function declaration with doc comments and `\d` number of arguments     | Empty line  |
| Regex      | hfuncc\d     | creates function prototype with doc comments and `\d` number of arguments       | Empty line  |

## Go

| type       | trigger | description                                                                | restriction |
| ---------- | ------- | -------------------------------------------------------------------------- | :---------: |
| Regex      | func\d  | Creates function declaration block with `\d` number of arguments           | Empty line  |
| Line Begin | struct  | create struct declaration with comments                                    |             |
| Regex      | meth\d  | Creates method declaration block with `\d` number of arguments             | Empty line  |
| Regex      | msi\d   | expands to `map[string]interface{}{}` with `\d` number of key-value inside |             |
| Regex      | logr\de | logrus error with fields with `\d` number of key value                     | Empty line  |
| Regex      | logr\di | logrus info with fields with `\d` number of key value                      | Empty line  |
| Regex      | logr\df | logrus non-exit fatal field with fields with `\d` number of key value      | Empty line  |
