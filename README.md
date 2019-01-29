# mac-tricks

Many commands can be found here: https://www.defaults-write.com/


## Change the icon size in stacks
Press `CMD +` or `CMD -` when the stack is open.

## Only show active apps
`defaults write com.apple.dock static-only -bool TRUE; killall Dock`
Source: https://www.makeuseof.com/tag/customise-mac-os-x-dock-hidden-terminal-commands/

## Enable “Single App” mode
`defaults write com.apple.dock single-app -bool TRUE; killall Dock`
Source: https://www.makeuseof.com/tag/customise-mac-os-x-dock-hidden-terminal-commands/

## Add custom stacks for recent, documents, and more
`defaults write com.apple.dock persistent-others -array-add '{"tile-data" = {"list-type" = 1;}; "tile-type" = "recents-tile";}'; killall Dock`
Source: https://www.makeuseof.com/tag/customise-mac-os-x-dock-hidden-terminal-commands/

## You can switch what a "Recent" stack shows, by choosing in the context menu. `Control + Click` on the stacks icon.

## Add application spacers
`defaults write com.apple.dock persistent-apps -array-add '{"tile-type"="spacer-tile";}'; killall Dock`
Source: https://www.makeuseof.com/tag/customise-mac-os-x-dock-hidden-terminal-commands/

## Indicate hidden app icons
`defaults write com.apple.dock showhidden -bool TRUE; killall Dock`
Source: https://www.makeuseof.com/tag/customise-mac-os-x-dock-hidden-terminal-commands/

## Change or disable Auto-HidedDelay
`defaults write com.apple.dock autohide-time-modifier -float 1; killall Dock`
The Number works as a multiplier.
Source: https://www.makeuseof.com/tag/customise-mac-os-x-dock-hidden-terminal-commands/

## Use scroll gestures (similar to Exposé)
`defaults write com.apple.dock scroll-to-open -bool TRUE; killall Dock`
Source: https://www.makeuseof.com/tag/customise-mac-os-x-dock-hidden-terminal-commands/

## Enable the hidden "Suck" animation
`defaults write com.apple.dock mineffect suck; killall Dock`
Possible animations are: "suck" to "genie" or "scale".
Source: https://www.makeuseof.com/tag/customise-mac-os-x-dock-hidden-terminal-commands/

## Enable hover-highlighting in the Dock-Stacks
`defaults write com.apple.dock mouse-over-hilite-stack -boolean yes;killall Dock`
Replace `yes`with `no`to reverse it.
Source: http://osxdaily.com/2008/01/07/highlight-stack-items-on-hover/

## Change the layout (rows and columns) of Launchpad
Set the columns count: `defaults write com.apple.dock springboard-columns -int X`
Set the rows count: `defaults write com.apple.dock springboard-rows -int X`
Restart the Dock after the changes: `killall Dock`
To Reset: Use the commands without `-int X`:
`defaults delete com.apple.dock springboard-rows; defaults delete com.apple.dock springboard-columns; killall Dock`
Source: https://www.defaults-write.com/change-the-layout-rows-and-columns-of-launchpad/

## To reset the whole Launchpad
`defaults write com.apple.dock ResetLaunchPad -bool TRUE; killall Dock`
Source: https://www.defaults-write.com/change-the-layout-rows-and-columns-of-launchpad/
