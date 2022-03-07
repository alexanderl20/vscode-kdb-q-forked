# Change Log

## 1.2.1 - Forked Version

New Features:

* crtl+enter used for both running line of code and running highlighted code
* Results returned even if line ends in semi-colon
* Results returned when assigning values
    * eg a:"test" will now return "test", where before it returned (::)
* Typing each-both ' does not result in quotes '' being created
* Code can be commented out using VSCode shortcut

Removed Features:

* Grid view 

Bug Fixes:

* Data displayed how it would in terminal + syntax
* All valid q code will run successfully


## 1.2.0

* Added support for printing dictionaries and keyed tables
* Added icon to status bar to indicate connection status
* Added auto (re)connect upon query
* Several bug fixes regarding query results
* Usability and interface improvements

## 1.1.2

* Minor fixes to grid view, and nested object formatting

## 1.1.1

* Added server view (configurable through settings.json)
* Minor fixes to how result views are handled

## 1.1.0

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

## 1.0.0

Initial release of vscode-kdb-q, featuring:

* Accurate syntax highlighting
* Reliable code completion (based on remote server process)
* Running kdb+ queries and output the result in a console
* Show table results in a high performance grid view
* Explorer view exposing all functions and variables