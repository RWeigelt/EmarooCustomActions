FAQ
===

What is Emaroo?
---------------

[Emaroo](http://roland-weigelt.de/emaroo) is a free utility for browsing most recently used (MRU) file lists of programs like Visual Studio, Word, Excel, PowerPoint and more. Quickly open files, jump to their folder in Windows Explorer, copy them (and their path) to the clipboard - or run your own tools on the MRU items! And all this with just a few keystrokes or mouse clicks.

What is a custom action?
------------------------

A custom action is call to an executable of your choice, with information about the currently selected file or directory.

You execute a custom action by clicking one of the buttons at the bottom of the list of most recently used item, pressing a Ctrl+_number_ hotkey or opening the context menu on a list item.

How do I use one of the custom actions in this repository?
----------------------------------------------------------

* _Either_ download/clone this repository and open the `.action.json` file for the custom action(s) you want from the `actions` folder
* _Or_ go to [the list of custom actions](README.md) and follow the instructions on the page.

How do I write my own custom action?
------------------------------------

* In Emaroo, open the Settings tab
* Select a tool/application in the list on the left
* Click the "+ Add New" button (or press `Ctrl+N`)
* Specify name, executable, arguments, etc.
* Click on the name of a macro to insert it. The macros work the same way as those in the custom build steps in Visual Studio (i.e. directory macros end on a backslash)

How do I contribute to the list of custom actions?
--------------------------------------------------

If you have a custom action that may be of interest to others,

* _either_ create a pull request
* _or_ send me the JSON file for the custom action via email (see the footer of the [Emaroo website](http://www.roland-weigelt.de/emaroo/))
