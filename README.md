## Outline for Sublime Text 3

##### Makes an outline of the code for quick navigation and orientation within a file.

![](assets/markdown-img-paste-20181008011255139.png?raw=true)

1. Forked and updated by Adam Tableman for UCLA/IST use. See [original repository](https://github.com/warmdev/SublimeOutline) for the base code on which this code is based/forked.
2. For Fortran, install the _Fortran+_ Sublime Text Plugin at [https://github.com/UCLA-Plasma-Simulation-Group/tools_sublimetext_fortran(https://github.com/UCLA-Plasma-Simulation-Group/tools_sublimetext_fortran)].  _Fortran+_ fixes a few issues in the Sublime's Fortran support and also makes changes so that the _Outline+_ plugin works better. If _Fortan+_ is installed, the outline will be as shown in the above screenshot with indentation and '----contains----' entries that show where Fortran _contains_ statements occur in the code.

### Installation
Just 4 easy steps!
1. __If you previously installed the _Outline_ package, you must uninstall it.__
2. __Add the _Outline+_ repository to Sublime Text's package manager:__
3. __Install Outline+__
4. __Turn on the outline__

If you are new to Sublime Text, see the _Installation Walkthrough_ section below for detailed instructions.

### Installation Walkthrough
1. __If you previously installed the _Outline_ package, you must uninstall it.__
    * Open Command Palate (Mac: &#8984;-Shift-P or Windows: Ctrl-Shift-P)
    * Type 'remove package' then select the 'Package Control: Remove Package' item.
    * Scroll though the list and select the _Outline_ item to uninstall it. (If you don't see an  _Outline_ entry it's no big deal... it just means  _Outline_ isn't installed which is what we were after anyway!)
    * ![](assets/remove_outline.gif?raw=true)
2. __Add the _Outline+_ repository to Sublime Text's package manager:__
    * Open Command Palate (Mac: &#8984;-Shift-P or Windows: Ctrl-Shift-P)
    * Type 'add repository' then select the 'Package Control: Add Repository' item.
    * Then paste in the value: `https://raw.githubusercontent.com/UCLA-Plasma-Simulation-Group/tools_sublimetext_outliner/master/info.json`
    * ![](assets/add_repo.gif?raw=true)
3. __Install Outline+__
    * Open Command Palate (Mac: &#8984;-Shift-P or Windows: Ctrl-Shift-P)
    * Type 'install package' then select the 'Package Control: Install Package' item
    * Type 'Outline+' then select the 'Outline+' item
    * ![](assets/install_package.gif?raw=true)
4. __Turn on the outline__
    * Open Command Palate (Mac: &#8984;-Shift-P or Windows: Ctrl-Shift-P)
    * Type 'outline'
    * Select one of the 5 layout options that come up:
        * 'Browse Mode: Outline (Left)'
        * 'Browse Mode: Outline (Right)'
            * This is one shown in the screenshot above.
        * 'Browse Mode: Filebrowser Left, Outline Right'
        * 'Browse Mode: Filebrowser Top Left, Outline Bottom Left'
        * 'Browse Mode: Filebrowser Top Right, Outline Bottom Right'
    * See the _Default layout_ section below for more info.
    * ![](assets/turn_on.gif?raw=true)
### Default layout  

The outline tab can be set as a sidebar on the left or right. Press `Ctrl + Shift + P` and select either `Browse Mode: Outline (Left)` or `Browse Mode: Outline (Right)` to set your preferred layout.

If you also use [FileBrowser](https://github.com/aziz/SublimeFileBrowser), you can use both in three different layouts:

* `FileBrowser` left, `Outline` right
* `FileBrowser` top left, `Outline` bottom left
* `FileBrowser` top right, `Outline` bottom right

To use `FileBrowser` and `Outline` together, please close the `FileBrowser` sidebar first and then use the correponding `Browse Mode` command to set the layout, otherwise the `Outline` view may not work as intended.

### Color theme

`Outline` has two built-in color themes: Bright (default theme) and Dark. To switch to the Dark theme, add the following to your user settings file. Open the user settings file by "Preferences > Package Settings > Outline > Settings" (Sublime Text version 3124 or later), or "Settings - User":

```json
"color_scheme": "Packages/Outline+/outline-Dark.hidden-tmTheme"
```

Remove `-Dark` or remove the entire line to return to the bright theme. To customize your own color theme, see [this issue](https://github.com/warmdev/SublimeOutline/issues/1).

### Outline content and indentation

Outline is updated when you save a file or switch between files.

Content and indentation in the `Outline` tab is controlled by the `Symbol List.tmPreferences` file (file name may differ) corresponding to the syntax of your file.

### Known issue

* This package may not work if you use a multi-column/row layout.

### License

This plugin is licensed under the MIT license.
