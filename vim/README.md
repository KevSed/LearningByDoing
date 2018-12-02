# ♥im unsorted list of briliant stuff

## Insert next non digit literally
```
see :h i_CTRL-V
```
Example:
^v Esc will produce ^[ which is represented in vim as esc character, same with Enter, Backspace, ...
This is very usefull when writing one line commands like:
```
:norm 0 i Hello^[AWorld.
```
This goes to every line and executes above command with Esc after Hello.
### ASCII Code
To insert ASCII Code just type ^v u 2665, which will produce ♥, where 2665 is ascii code for a heart.


## Ctrl-X
Amazing keywork completion.
Example:
```
" In insert mode you see this text:
^v Esc
" Type ^X ^L still in insert mode will produce this
" by completing whole text by already seen text
^v Esc will produce ^[ which is represented in vim as esc character, same with Enter, Backspace, ...
" Type ^X ^L again and you will also get the next line
^v Esc will produce ^[ which is represented in vim as esc character, same with Enter, Backspace, ...
This is very usefull when writing one line commands like:
```
There are plenty more completion modes then ^L.

## Clipboard action
###Copy to system clipboard
Vim needs to be compiled with system clipboard access
```
"* Y
```
Yanks line in register \*, which is system clipboard. (Might also be + instead of \*)
