# vscode-kdb-q-forked

This is a forked version of [xidaozu's](https://github.com/real-xidaozu/vscode-kdb-q) extension [vscode-kdb-q]](https://marketplace.visualstudio.com/items?itemName=xidaozu.vscode-kdb-q) - V1.2.0.


This README will only contain changes made from the [original](https://github.com/real-xidaozu/vscode-kdb-q).


## Keyboard Shortcuts

| Keyboard shortcut                                  | Command                                                            |
| ---------------------------------------------------| ------------------------------------------------------------------ |
| <kbd>Ctrl</kbd>/<kbd>Cmd</kbd> + <kbd>Enter</kbd>  | If code is highlighted then run it, else run current line as query |



## Sublime Syntax highlighting

This is personal preference, sublime syntax:
* has different colours for symbols, .Q namespaces and built in functions
* has highlighting for assigning variables


Original:

![image](https://user-images.githubusercontent.com/92346145/156467735-8c9adb7c-af02-4e30-b7cb-3d96d1ba0825.png)


New:

![image](https://user-images.githubusercontent.com/92346145/156467756-effb8a0a-a6f7-457d-9af7-8c77cc401c55.png)





## QoL Improvements

* Any trailing semicolons in code are removed at execution to allow results to be returned
* Assigning values to variable will still return data (eg a:"test" will now return "test", where before it returned (::))
* typing each-both ' does not result in quotes '' being created


## Bug Fixes 

* Symbols can now be queried and not error out
* Strings appear as correct syntax  
* console size can be adjusted as expected, min size set to 20 200
