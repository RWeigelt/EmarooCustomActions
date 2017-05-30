EmarooCustomActions
===================
Custom actions for [Emaroo](http://roland-weigelt.de/emaroo), the free utility for browsing the most recently used lists of tools and applications like Visual Studio, Word, Excel, PowerPoint and more.

What is a custom action?
------------------------

A custom action is call to an executable of your choice, with information about the currently selected file or directory.

You execute a custom action by clicking one of the buttons at the bottom of the list of most recently used item, pressing a Ctrl+_number_ hotkey or opening the context menu on a list item.

How do I use one of the custom actions in this repository?
----------------------------------------------------------

* _Either_ download/clone this repository and open the `.action.json` file for the custom action(s) you want from the `actions` folder
* _Or_ go to **[the list of custom actions](actions/Actions.md)** and follow the instructions on the page.

How do I write my own custom action?
------------------------------------

* In Emaroo, open the Settings tab
* Select a tool/application in the list on the left
* Click the "+ Add New" button (or press `Ctrl+N`)
* Specify name, executable, arguments, etc.
* The macros work the same way as those in the custom build steps in Visual Studio (i.e. directory macros end on a backslash)
