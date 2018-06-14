Custom Actions for Emaroo 4
=========================

A custom action for [Emaroo](https://www.roland-weigelt.de/emaroo/) calls an executable with arguments built using macros e.g. for the full path of currently selected file/directory, or just the file name, the extension, etc.

Custom actions are defined per-application. They appear as buttons below the corresponding list of most recently used (MRU) items and as entries of the  item's context menu. If you prefer hotkeys, you can also run a custom action via <kbd>Ctrl</kbd>+_number_.

(_The custom actions for Emaroo 3.x [have been moved below the `v3` folder](v3/README.md)_)

Sharing Custom Actions
---

Starting with Emaroo 4, custom actions can be shared by copying/pasting a text string that you can put on an HTML page, insert into an email, or maybe even post on Facebook ;-).

File-based import/export of individual custom actions (via `.action.json` files) is still supported and will continue to be in the future.

Ready-to-use Custom Actions
---
The custom actions are categorized by the executable that is _called_:
* [Visual Studio](actions/visualStudio.md)
* [Visual Studio Code](actions/code.md)
* [Tools related to Git](actions/git.md)
* [Applications for designers](actions/designers.md)
* [Other applications/tools](actions/misc.md)

How to Use
---
As an example, here's a custom action that creates a new mail in Outlook and adds the current file as an attachment (read how it was done in "[How to Write Your own Custom Action](WriteYourOwn.md)"):
```
§§!F5[*J,m1]zzYr^^u1xKwvI-6rj=lP}5A7qkrB|w(AO9,y3lagyKpe)efm%4SDV*gH+°wlT[|^i^Sg
0{HMG^JV;GvLqWf]fVqk_O9vg)MHopIIP?xmhZZy|0h9=3-6q87B$)%r2W%UDdE26W*%q2g)NVXser^1
P{n-gB8r5°Ny:KnO4#[q(lpwv-o6W.iH-!06EGAv,dv,%Mb6k]$0EP*,wIih;A§§
```
* Select and copy the text for the custom action to the
  clipboard.
* In Emaroo, open the Settings tab ( ![](_images/ConfigTabIcon.png) ).
* In the "Applications" list on the, select the tool/application you want to add the custom action to:
  ![](_images/CustomAction_SelectApplication.png)
* In the "Custom Actions for ..." list, click the "Paste" button (or press <kbd>Strg</kbd>+<kbd>V</kbd>) to paste the custom action.
  ![](_images/CustomAction_AfterPasting.png)
* Switch back to the application's tab page and you're good to go!
* **Tip:** You can view the custom action for a specific selected file or folder before running the custom action by opening the context menu on the custom action's button and selecting "Debug":
  ![](_images/CustomAction_Debug.png)
* In the debug dialog you'll see the actual command line to be used (and you can inspect the values of all macros):
  ![](_images/CustomAction_DebugDialog.png)

  Want to Write Your Own?
  ---
  Take a look at "[How to Write Your own Custom Action](WriteYourOwn.md)"!