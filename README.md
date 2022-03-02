# vscode-kdb-q-forked

This is a forked version of [xidaozu's](https://github.com/real-xidaozu/vscode-kdb-q) extension [vscode-kdb-q]](https://marketplace.visualstudio.com/items?itemName=xidaozu.vscode-kdb-q) - V1.2.0.


This README will only contain changes made from the [original](https://github.com/real-xidaozu/vscode-kdb-q).


## Keyboard Shortcuts

| Keyboard shortcut                                  | Command                                                            |
| ---------------------------------------------------| ------------------------------------------------------------------ |
| <kbd>Ctrl</kbd>/<kbd>Cmd</kbd> + <kbd>Enter</kbd>  | If code is highlighted then run it, else run current line as query |



## Sublime Syntax highlighting

Personal preference, has highlighting for symbols and knows the difference between kdb-specific and custom namespaces



## QoL Improvements

* Any trailing semicolons in code are removed at execution to allow results to be returned
* Assigning values to variable will still return data (eg a:"test" will now return "test", where before it returned (::))
* typing each-both ' does not result in quotes '' being created


## Bug Fixes 

* Symbols can now be queried and not error out
* Strings appear as correct syntax  
* console size can be adjusted as expected, min size set to 20 200















This [Visual Studio Code extension](https://marketplace.visualstudio.com/items?itemName=xidaozu.vscode-kdb-q) provides extensive features for the [kdb+/q](https://code.kx.com/q/) programming language.
Features include syntax highlighting, auto completion, executing queries on a kdb+ server, table visualization and more.
The extension is developed with Atom's [connect-kdb-q](https://github.com/quintanar401/connect-kdb-q) extension and [QInsightPad](http://www.qinsightpad.com/) in mind.
Although any theme will work, the recommended theme is [Atom One Dark](https://marketplace.visualstudio.com/items?itemName=akamud.vscode-theme-onedark) for the best experience.

Please note that the extension is usable in its current state, but is still under development.

## Features

The extension currently provides the following features:

* Accurate syntax highlighting
* Reliable code completion (based on remote server process)
* Running kdb+ queries and output the result to multiple views
* Syntax highlighted document view for query results
* High performance grid view for table results
* Console view supporting even the largest table sizes 
* Explorer view exposing all functions and variables
* Server view configurable per workspace (settings.json)

## Demonstration 

![Demo](https://github.com/real-xidaozu/real-xidaozu.github.io/blob/master/img/static/vscode-kdb-q-demo.gif?raw=true)

## Requirements

VS Code 1.47.0 is required and kdb+ 3.6 or higher is recommended.

## Extension Settings

| Name                                | Default    | Description                                              |
| ------------------------------------| ---------- | -------------------------------------------------------- |
| `vscode-kdb-q.consoleViewEnabled`   | `false`    | Whether results should be printed to the kdb-q console   |
| `vscode-kdb-q.gridViewEnabled`      | `true`     | Whether table results should be printed to the grid view |
| `vscode-kdb-q.documentViewEnabled`  | `true`     | Whether results should be printed to a virtual document  |
| `vscode-kdb-q.gridViewPosition`     | `Two`      | The view column used show the grid view                  |
| `vscode-kdb-q.documentViewPosition` | `Grid`     | The view column used show the document view              |
| `vscode-kdb-q.serverList`           | `[]`       | Array with server connection strings (`host:port:id:pw`) |
| `vscode-kdb-q.serverGroupMode`      | `Hostname` | The rule for server grouping withing the server view     |

## Keyboard Shortcuts

| Keyboard shortcut                                                | Command                      |
| ---------------------------------------------------------------- | ---------------------------- |
| <kbd>Ctrl</kbd>/<kbd>Cmd</kbd> + <kbd>Q</kbd>                    | Connect to kdb+ server       |
| <kbd>Ctrl</kbd>/<kbd>Cmd</kbd> + <kbd>E</kbd>                    | Run selection as query       |
| <kbd>Ctrl</kbd>/<kbd>Cmd</kbd> + <kbd>Enter</kbd>                | Run current line as query    |

## Known Issues

Below is a list of known issues and incomplete features:

* Code completion is not supported when not connected to a kdb+ server
* Nested table objects are not printed to console/document view

## License

Licensed under GNU General Public License v3.0.
See the license file for more details.

## Release Notes

### 1.2.0

* Added support for printing dictionaries and keyed tables
* Added icon to status bar to indicate connection status
* Added auto (re)connect upon query
* Several bug fixes regarding query results
* Usability and interface improvements

### 1.1.2

* Minor fixes to grid view, and nested object formatting

### 1.1.1

* Added server view (configurable through settings.json)
* Minor fixes to how result views are handled

### 1.1.0

New features:

* Syntax highlighted document view for query results
* Extension settings for enabled panels and their positions
* Click items from kdb+ explorer to see their contents
* Default keybindings (Ctrl+Q for connect, Ctrl+E/Ctrl+Enter for running queries)
* Support for filtering dates and numbers in grid view
* Connection status bar item is now clickable to connect
* Nanosecond precision for timespans (up from milliseconds)
* Microsecond precision for timestamps (up from milliseconds)

Bug fixes:

* Fixed auto completion not working in some cases
* Fixed printing of empty tables
* Fixed variables in global namespace in kdb+ explorer

### 1.0.0

Initial release of vscode-kdb-q.
