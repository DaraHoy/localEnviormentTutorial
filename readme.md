# Setup a Local Enviorment

## Install Git BASH
  1. Go to <https://git-scm.com/download> to download the latest version of Git BASH.
  2. Follow the the install prompts, clicking next on all default options.

## Install Node.js
  1. Go to <https://nodejs.org/> to download the latest version of Node.
  2. Follow the the install prompts, clicking next on all default options.

## Choose a text editor
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

**For the purposes of this walkthrough we'll be utilizing VSCode*

## Install VSCode 
 1. Go to <https://code.visualstudio.com> download the latest version.
 2. Follow the the install prompts, clicking next on all default options.
 ### Select Git BASH as your default terminal 
 3. Open the Command Pallet
 ``` ctrl + shift + p ```
 4. Type 'Select Default Shell', select Git Bash

## Create a new SSH Key
1. Toggle your terminal with `ctrl + \`` 
2. Paste the text below, substituting in your GitHub email address.
``` ssh-keygen -t rsa -b 4096 -C "your_email@example.com" ```
This creates a new ssh key, using the provided email as a label.
``` Generating public/private rsa key pair. ```
3. When you're prompted to "Enter a file in which to save the key," press Enter. This accepts the default file location.
``` Enter a file in which to save the key (/c/Users/you/.ssh/id_rsa):[Press enter] ```
4. At the prompt, type a secure passphrase. For more information, see "Working with SSH key passphrases".
```
Enter passphrase (empty for no passphrase): [Type a passphrase]
Enter same passphrase again: [Type passphrase again]
```
5. Adding your SSH key to the ssh-agent, type 
```$ eval $(ssh-agent -s)```
6. Add your SSH private key to the ssh-agent. If you created your key with a different name, or if you are adding an existing key that has a different name, replace id_rsa in the command with the name of your private key file.
```$ ssh-add ~/.ssh/id_rsa```
7. Copy the SSH key to your clipboard.
```$ clip < ~/.ssh/id_rsa.pub```
8. Go to your <https://github.com/settings/profile> and click SSH and GPG keys
9. Click Click New SSH Key or Add SSH Key.
10. Give your key a descriptive label-e.g., 'Dara's Macbook'.
11. Paste your key into the "Key" field and click Add SSH key
12. If prompted, confirm your GitHub password.

## Test a commit
1. Navigate to your desktop inside VSCode terminal and create a folder called test `$ mkdir test`
2. cd into /test and initialize Git `$ git init`
3. Create a new file `$ touch index.js`
4. Open the file in VSCode `$ code index.js`
5. Add a `console.log('Hello World!')` line and save
6. In the terminal add the file and write a commit message
```
$ git add -A
$ git commit -m 'Add hello world'
```
7. Go to <https://github.com/new> and create a new repository called test, no need to add a gitignore or license. 
8. Copy the git remote add origin line and paste into your terminal.
9. Enter `git push -u origin master`
