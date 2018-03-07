# Setup a Local Enviorment

## Install Git BASH
  1. Go to <https://git-scm.com/download> to download the latest version of Git BASH.
  2. Follow the the install prompts, clicking next on all default options.

## Install Node.js
  1. Go to <https://nodejs.org/> to download the latest version of Node.
  2. Follow the the install prompts, clicking next on all default options.

## Available modern text editors
There are many text editors available that can write code for Node.js:
* Atom
* Brackets
* Coda 
* Sublime Text
* Vim
* Emacs
* ~~Notepad++~~ 

### Recommended editor
#### Visual Studio Code
* Maintained and developed by Microsoft
* Fast & polished
* Extensions library
* Debugger
* Git support
* Terminal
* Built on Node.js

*For the purposes of this walkthrough we'll be utilizing VSCode*

## Install VSCode 
 1. Go to <https://code.visualstudio.com> download the latest version.
 2. Follow the the install prompts, clicking next on all default options.
 ### Select Git BASH as your default terminal 
 3. Open the Command Pallet
 ``` ctrl + shift + p ```
 4. Type 'Select Default Shell', select Git Bash

## Setup a SSH key with GitHub 
1. Toggle your terminal with ctrl + ` 
2. Navigate to your desktop and create a folder called test `$ mkdir test`
3. Inside /test initialize Git `$ git init`
4. /test create a file `$ touch index.js`
5. Open the file in VSCode `$ code index.js`
6. Add a `console.log('Hello World!')` line and save
7. Git add the file and write a commit message
```
$ git add -A
$ git commit -m 'Add hello world'
```
8. Go to <https://github.com/>
### Creating a SSH Key 

