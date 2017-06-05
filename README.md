Custom Actions for Emaroo
=========================

### To import an individual custom action...

* Copy the link URI of the custom action you want to use to the clipboard.
* Start Emaroo, open the Settings tab ( ![](_images/ConfigTabIcon.png) ).
* In the "Applications" list, select the tool/application you want to add the custom action to.
* In the "Custom Actions for ..." list, press the "Import" button ( ![](_images/CustomAction_Import.png) ).
* On the "Open File" dialog, paste the URI you copied before, click the "Open" button.

### To import a collection of custom actions...

* Copy the link URI of the config file.
* Start Emaroo, open the Settings tab ( ![](_images/ConfigTabIcon.png) ).
* In the lower left corner, press the "Import" button ( ![](_images/Config_Import.png) ).
* On the "Open File" dialog, paste the URI you copied before, click the "Open" button.
* In the import dialog, you'll see how your configuration will look after the import, look for "Add"

**BEFORE RUNNING A CUSTOM ACTION, ALWAYS REVIEW WHAT IT WILL DO!!**

[Questions? The FAQ is here to help!](FAQ.md)

---

Visual Studio
-------------

### Developer Command Line

Opens the developer commandline for Visual Studio (@RWeigelt)

#### Individual custom actions
* Visual Studio 2017 - [**Link**](https://raw.githubusercontent.com/RWeigelt/EmarooCustomActions/master/visualStudio/Developer%20CMD%20(2017).action.json)
* Visual Studio 2015 - [**Link**](https://raw.githubusercontent.com/RWeigelt/EmarooCustomActions/master/visualStudio/Developer%20CMD%20(2015).action.json)
* Visual Studio 2013 - [**Link**](https://raw.githubusercontent.com/RWeigelt/EmarooCustomActions/master/visualStudio/Developer%20CMD%20(2013).action.json)
* Visual Studio 2012 - [**Link**](https://raw.githubusercontent.com/RWeigelt/EmarooCustomActions/master/visualStudio/Developer%20CMD%20(2012).action.json)
* Visual Studio 2010 - [**Link**](https://raw.githubusercontent.com/RWeigelt/EmarooCustomActions/master/visualStudio/Developer%20CMD%20(2010).action.json)

<!--
#### Collection

* Visual Studio 2010-2017 - [**Link**]()
-->

**Note:** The custom actions use the `$(ExeDirPath)` macro to honor the installation path of Visual Studio. If you want to use one of these custom actions on another application/tool's MRU list, you have to use an absolute path matching your system.

---

Developer Tools
---------------

### Hg Workbench - [**Link**](https://raw.githubusercontent.com/RWeigelt/EmarooCustomActions/master/misc/Hg%20WorkBench.action.json)

Opens the Hg Workbench of [TortoiseHg](https://tortoisehg.bitbucket.io/) in the current directory (@RWeigelt)

---