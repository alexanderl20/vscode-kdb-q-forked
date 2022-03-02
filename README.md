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


|Original                                                                                                       |Sublime                                                                                                        |
|---------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------|
|![image](https://user-images.githubusercontent.com/92346145/156468768-a2f79b2d-2a17-4fac-97f8-3b48da41b97a.png)|![image](https://user-images.githubusercontent.com/92346145/156468786-d41aa062-1c1a-4fa2-a4f1-c35e9ecb1913.png)|





## QoL Improvements

* Any trailing semicolons in code are removed at execution to allow results to be returned
* Assigning values to variable will still return data (eg a:"test" will now return "test", where before it returned (::))
* typing each-both ' does not result in quotes '' being created


## Bug Fixes 

* Symbols can now be queried and not error out
* Strings appear as correct syntax  
* console size can be adjusted as expected, min size set to 20 200
