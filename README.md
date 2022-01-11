# firefox-css
Firefox CSS customization

Firefox CSS code to remove some of the bloat that comes with the vanilla version.

## Prequisite:
Unlock custom CSS usage

`about:config` > `toolkit.legacyUserProfileCustomizations.stylesheets` > `true`  


### How to use:
Copy the userChrome.css file or contents into your Firefox profile's **chrome** folder. Create the folder if it does not exist.
Find the profile by going to about:support then clicking **Open Directory**

* Typical linux location: ~/.mozilla/firefox/####.default/chrome
* Typical Windows location: %APPDATA%\Mozilla\Firefox\Profiles\

### What is removed:
* Send Link to Device (and separator)
* Send Page to Device (and separator)
* Send, Copy, Set Image as background
* Bookmark Link

### Other stuff to remove
Some stuff can be removed by disabling extensions. open about:config and disable as desired:
* extensions.pocket.enable;false
* extensions.screenshots.disabled;true

### How to find item ids and attributes?

Enable once:
1. Tools > WebDeveloper > Toggle Tools > Toolbox Options > Enable browser chrome and add-on debugging toolboxes
2. Tools > WebDeveloper > Toggle Tools > Toolbox Options > Enable remote debugging

Hit Ctrl+Alt+Shift+I or open 'Tools > WebDeveloper > Browser Toolbox'.

Inspect ui or web content.

Force popups to stay open for inspection:
Click on 'disable popup auto hide' button (= button with four squares) on developer toolbars end.

### References
* Element names and IDs: https://github.com/Aris-t2/CustomCSSforFx
