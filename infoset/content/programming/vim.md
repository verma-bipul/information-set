---
title: "Vim"
date: 2022-11-16T10:51:27-06:00
draft: false
---

## Basic Editing with Vim 

Vim is a powerful text editor designed in such a manner such that one has to never leave the keyboard. So here are some basics.

There are three basic modes: (i) the command mode, (ii) the insert or edit mode, (iii) last line mode. The command mode is basically to browse through the files. This is the mode the file will open as default. In this mode one can't edit the file. To edit the mode one has to go to the insert mode by pressing the `i' key. The last line mode is where we enter the commands to save files or perform other functionalities.

## Basic Navigation 

- h, j, k, l are used to navigate the pointer left, down,up and right.    
- w, b are used to move between words    
- 0, $ to move between beginning, and end of line    
- gg, G to move to beginning, and end of file     
- ZZ to save and exit.     
- e to move cursor to the end of line   
- 20G to jumps to line 20 in vim    

## Scrolling in Vim
ctrl+d: scroll down     
ctrl+u: scroll up    
ctrl+f: one page forward    
ctrl+b: one page backward    

## Insert Mode positioning 
There are several keys to jump to insert mode. The following is a list of keys with their functionality.
Note: By default everything is typed to the left of cursor.     
i - will begin the insert mode at the current position of the cursor    
a - will begin the insert mode by placing cursor to one character to the right    
I - append at the beginning of a line          
A - append at the end of a line    

## Delete Functionalities:
- d starts the delete operation. Once we have entered this operation the navigation h,j,k, l will still be operational.
- d followed by the standard line jumping keys will implement delete for those commands. For instance:
- d0, d$, dgg, dG, deletes to the beginning, end
- x  delete character

Note: The detele functionality is the same as cutting the text. It is temperorily stored in the buffer.


## Copy and pasting
The basic idea here is to enter the selection mode using v or V. Once we are in the selection mode, we can use the usual navigation tools to select the desired texts. V will select by line, v by words.
The letter 'y' which stands for yank copies the selected text to the buffer. To paste the selcted text, just use 'p'.    
To cut and paste in the visual mode one can use 'd' followed by 'p'. 


## Working on Multiple files using Vim



## Some other useful commands 

-  To push vim to the background and return to the terminal we do 'ctrl+z'. To come back we just type 'fg'.   
- To display line number we use ':set number' or ':set nu' in short.  

### Split Screen functionality
- In order to open multiple files in split screen at the same time use the command  vi -o file1 file2'. By default it will open files in a horizontal split.
- To toggle between the horizontal screens we use the 'ctrl + w' followed by j to move down and k to move up to move down and k to move up. The up and down keys works as well.
- Similarly 'ctrl+ w' followed by h, l moves to left and right or one can simply use the cursor keys as well.
- To adujst the size of the splits: 'ctrl+W' + = : equal horizonatal splits. 



## Plugin Manager in Vim 
www.linuxhandbook.com/install-vim-plugins/    
 



## Vim Configurations   
Vim configrations are saved in the `~/.vimrc` configration file.   

One can add the follwing functionalites which will be active from the start.    
```vim
 set number - this displays the line numbers
```


## Spell check in Vim
- Simply add `set spell` in the config file.     
- [s or ]s are used to navigate between the misspelled words.
- z= will give a list of suggested words.

References:    
1. https://www.linuxfoundation.org/blog/blog/classic-sysadmin-vim-101-a-beginners-guide-to-vim    
2. https://linuxhint.com/vim_split_screen/   -- this is regarding split functionalities.     
  
