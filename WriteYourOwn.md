How to Write Your own Custom Action
===
Let's say, you want to write a custom action that creates a new mail in Outlook and adds the current file as an attachment. For this walkthrough we'll start writing the custom action for Excel, but of course we're able to copy the action to other applications later.

* In Emaroo, open the Settings tab ( ![](_images/ConfigTabIcon.png) ).
* In the "Applications" list on the, select the tool/application (in this case Excel):  
  ![](_images/CustomAction_SelectApplication.png)
* In the "Custom Actions for ..." list, click the "Add new" button (or press <kbd>Strg</kbd>+<kbd>N</kbd>) to create a new custom action:  
  ![](_images/CustomAction_Example1.png)
* Let's choose a short name:  
  ![](_images/CustomAction_Example2.png)
* Next, we need to specify the executable. The idea is to use Outlook, and it would be easy to use the "Browse..." button to specify the absolute path of `outlook.exe`. Instead, we'll use the text macros of Emaroo (which are similar to those in the build events of Visual Studio). While Emaroo doesn't know the full path of Outlook's executable, it _does_ know the full path of Word's (and `word.exe` is in the same folder as `outlook.exe`). So let's open the context menu on the "Executable" input field...  
  ![](_images/CustomAction_Example3.png)
* ...and use the "ExeDirPath" macro. To maximize portability across computers, we'll use the newest version of Word instead of a specific one:  
  ![](_images/CustomAction_Example4.png)
* In the arguments, we'll use some Outlook command line parameters to do the magic. The `/a` parameter specifies the file to be attached, so we'll need another macro here:  
  ![](_images/CustomAction_Example5.png)
* If you look at the full command line, you'll get an idea how to build command lines:  
  ![](_images/CustomAction_Example6.png)
* For this custom action, we don't need to specify a workind directory, so we'll skip the "Start in" input field.  
* A proper tooltip for the custom action would be nice, so let's click the "Tooltip" expander and enter some text:  
  ![](_images/CustomAction_Example7.png)
* Done!  
  ![](_images/CustomAction_Example8.png)
* Press "OK" to close the dialog and you'll see the custom action in the list:
  ![](_images\CustomAction_AfterPasting.png)

Copy/Paste
---
* Click the "" icon or press <kbd>Ctrl</kbd>+<kbd>C</kbd> to copy the custom action to the clipboard.
* You can now select another application in the "Applications" list...  
  ![](_images/CustomAction_SelectAnotherApplication.png)  
  and paste the custom action there.
* Or you paste the custom action into a text editor, an email, etc. to share it with others. The custom action described above looks like this:  
  ```
  §§!F5[*J,m1]zzYr^^u1xKwvI-6rj=lP}5A7rIT~2OWyd7#[|.?F1QjEF°V?K-sg276xlm#s7_~C.f;O
  E,FEFS=yc2yJq°xIo.$LqWHg$XYP$bK]3Xn5:B32EV_Zxc|,jWX=Ko)8m;XcL1XZvqeO;hu?p!-G,Tls
  16°w!awPY:#$%x-98[BP*Ky+?KJk2Cw=Vu-J5y0j?F28:xK=UIf_u(!swLtZ2a§§
  ```
