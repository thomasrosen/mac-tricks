# mac-tricks





# Dock

## Change the icon size in stacks: `CMD +` or `CMD -`

## Only Show Active Apps
`defaults write com.apple.dock static-only -bool TRUE; killall Dock`
Source: https://www.makeuseof.com/tag/customise-mac-os-x-dock-hidden-terminal-commands/

## Enable “Single App” Mode
`defaults write com.apple.dock single-app -bool TRUE; killall Dock`
Source: https://www.makeuseof.com/tag/customise-mac-os-x-dock-hidden-terminal-commands/

## Add Custom Stacks for Recent, Documents, and More
`defaults write com.apple.dock persistent-others -array-add '{"tile-data" = {"list-type" = 1;}; "tile-type" = "recents-tile";}'; killall Dock`
Source: https://www.makeuseof.com/tag/customise-mac-os-x-dock-hidden-terminal-commands/

## You can switch what a "Recent" Stack shows, by choosing in the context menu. `Control + Click` on the Stacks icon.

## Add Application Spacers
`defaults write com.apple.dock persistent-apps -array-add '{"tile-type"="spacer-tile";}'; killall Dock`
Source: https://www.makeuseof.com/tag/customise-mac-os-x-dock-hidden-terminal-commands/

## Indicate Hidden App Icons
`defaults write com.apple.dock showhidden -bool TRUE; killall Dock`
Source: https://www.makeuseof.com/tag/customise-mac-os-x-dock-hidden-terminal-commands/

## Change or Disable Auto-Hide Delay
`defaults write com.apple.dock autohide-time-modifier -float 1; killall Dock`
The Number works as a multiplier.
Source: https://www.makeuseof.com/tag/customise-mac-os-x-dock-hidden-terminal-commands/

## Use Scroll Gestures (similar to Exposé)
`defaults write com.apple.dock scroll-to-open -bool TRUE; killall Dock`
Source: https://www.makeuseof.com/tag/customise-mac-os-x-dock-hidden-terminal-commands/

## Enable the Hidden "Suck" Animation
`defaults write com.apple.dock mineffect suck; killall Dock`
Possible animations are: "suck" to "genie" or "scale".
Source: https://www.makeuseof.com/tag/customise-mac-os-x-dock-hidden-terminal-commands/
