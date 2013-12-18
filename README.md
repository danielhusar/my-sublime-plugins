My sublime plugins
==================

- All Autocomplete (will break colon after css autocomplete when there is empty lien before)
- Alignment
- DocBlockr
- Abacus
- Grunt
- Hayaku (will break css autocomplete values)
- HTMLBeautify
- Inc-Dec-Value
- JavaScript Snippets
- jQuery
- Less
- Sass
- Sublimelinter
- Theme - Soda
- VCS Gutter
- WordHighlight
- Sidebar enchancements
- BracketHighligher
- Browser refresh
- Dotfiles syntax highlighting
- Terminal
- Emmet
- Colorpicker
- Mou.app markdown


Sync between devices
====================


1. Quit Sublime Text 2 (so you don’t accidentally change any settings)
2. In your Dropbox folder (usually at ~/Dropbox/), add a folder called Sublime Text 2
3. Open the folder with your ST2 settings (should be ~/Library/Application Support/Sublime Text 2/)
4. Copy the following 3 folders into ~/Dropbox/Sublime Text 2/: Installed Packages, Packages, and Pristine Packages
5. Rename the original 3 folders in ~/Library/Application Support/Sublime Text 2/ to something like Installed Packages-20110119, Packages-20110119, and Pristine Packages-20110119 (optional, but I’m kind of anal about these things, so I want to make sure I can revert if need be)
6. Now, dive into Terminal.app (if you’re not comfortable using a CLI, you probably aren’t a good candidate for ST2)
7. Navigate into ~/Library/Application\ Support/Sublime\ Text\ 2/ (using cd, you got this, right?)
8. Here, we’re going to create symlinks to the folders in ~/Dropbox/Sublime Text 2/
9. The command to create a symlink is ln -s [source] [destination], so we want to do the following, 1 at a time:
(change the dropbox location)

```
  ln -s ~/Dropbox/_sync/Sublime\ Text\ 2/Installed\ Packages ./Installed\ Packages
  ln -s ~/Dropbox/_sync/Sublime\ Text\ 2/Packages ./Packages
  ln -s ~/Dropbox/_sync/Sublime\ Text\ 2/Pristine\ Packages ./Pristine\ Packages
```


Shortcuts
=========

- cmd + b - create minified version
- cmd + ctrl + x - add prefixes to css
- ctrl + g - go to line
- alt + up/down arrows - increnemt/decerement values
- ctrl + h - search the dash docset
- cmd + ctrl + j - pretty json
- cmd + shift + d - duplicate line
