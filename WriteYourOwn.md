How to Write Your own Custom Action
===
Let's say, you want to write a custom action that creates a new mail in Outlook and adds the current file as an attachment. For this walkthrough we'll start writing the custom action for Excel, but of course we're able to copy the action to other applications later.

* In Emaroo, open the Settings tab ( ![](_images/ConfigTabIcon.png) ).
* In the "Applications" list on the, select the tool/application (in this case Excel):  
  ![](_images/CustomAction_SelectApplication.png)
* In the "Custom Actions for ..." list, click the "Add new" button (or press <kbd>Strg</kbd>+<kbd>N</kbd>) to create a new custom action:  
  ![](_images\CustomAction_Example1.png)
* Let's choose a short name:  
  ![](_images\CustomAction_Example2.png)
* Next, we need to specify the executable. The idea is to use Outlook, and it would be easy to use the "Browse..." button to specify the absolute path of `outlook.exe`. Instead, we'll use the text macros of Emaroo (which are similar to those in the build events of Visual Studio). While Emaroo doesn't know the full path of Outlook's executable, it _does_ know the full path of Word's (and `word.exe` is in the same folder as `outlook.exe`). So let's open the context menu on the "Executable" input field...  
  ![](_images\CustomAction_Example3.png)
* ...and use the "ExeDirPath" macro. To maximize portability across computers, we'll use the newest version of Word instead of a specific one:  
  ![](_images\CustomAction_Example4.png)
* In the arguments, we'll use some Outlook command line parameters to do the magic. The `/a` parameter specifies the file to be attached, so we'll need another macro here:  
  ![](_images\CustomAction_Example5.png)
* If you look at the full command line, you'll get an idea how to build command lines:  
  ![](_images\CustomAction_Example6.png)
* For this custom action, we don't need to specify a workind directory, so we'll skip the "Start in" input field.  
* A proper tooltip for the custom action would be nice, so let's click the "Tooltip" expander and enter some text:  
  ![](_images\CustomAction_Example7.png)
* Done!  
  ![](_images\CustomAction_Example8.png)
* Press "OK" to close the dialog and you'll see the custom action in the list:
  ![](_images\CustomAction_AfterPasting.png)

Copy/Paste
---
* Click the "" icon or press <kbd>Ctrl</kbd>+<kbd>C</kbd> to copy the custom action to the clipboard.
* You can now select another application in the "Applications" list...  
  ![](_images\CustomAction_SelectAnotherApplication.png)  
  and paste the custom action there.
* Or you paste the custom action into a text editor, an email, etc. to share it with others. The custom action described above looks like this:  
  ```
  §§²lXkT!$qXGz!!#0°PY,qSN1"%COZ:³47"O0r9S#N@)-iIT)k/3RFj-nt_*^SIUe;l(_%-:G'S[,_C,
  lpZh6Mr*h^S\Z]/96DX:26]"_oqKgs0Atl_rXV\E\8AlP#7-`ZXN9N4t\h0;%UY`Y!g%k5EFr°U"1C_F
  ;h6,\`f0,2S4$:@K³MSO3Rif)[8a@f'a[ARTsTq?ZcgNYQAE\l6PHdDspcil"G+9sChD)lC[F:\Ql\K6
  (3b,O1.HZgPSB78a5C[LV\hl:7/5!ufA\T=g76@uO2WaiLL40`V§§
  ```