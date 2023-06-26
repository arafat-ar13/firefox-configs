# firefox-configs

I have started to use Firefox as my primary browser and this repository contains all of my Firefox configs and instructions. These are to be followed whenever a new Firefox installation occurs on any new device.

## Setup user.js file

I use [Betterfox](https://github.com/yokoffing/Betterfox) to "harden" my Firefox installation so that by default things like Mozilla telemetry, trackers, etc. are blocked by default for a more private browsing experience. Betterfox is convenient for me in the sense that it does not cause breakages and works as intended.

* Go to `about:config` on Firefox and check out which profile is current active. 
* Open the `root directory`.
* Copy and paste the `user.js` file into that folder

This `user.js` file comes directly from Betterfox, but it also has some [Betterfox common overrides](https://github.com/yokoffing/Betterfox/issues/87). The following have been overridden to be enabled:

* Firefox Account syncing
* Form and Address autofills
* Search suggestions on the URL box (it's okay since I use Brave Search)
* Google Safe Browsing

## Smoothfox: Edge-like Scrolling

Betterfox also provides an Edge-like smooth scrolling experience on Firefox. They have a custom JS file called [Smoothfox](https://github.com/yokoffing/Betterfox/blob/master/Smoothfox.js) that enables this feature. To enable it:

* Go to your `user.js` file
* In the Smoothfox section (below "SECTION: SMOOTHFOX"), add all the code from the Smoothfox.js file.

It really is just as good as Edge.

## Vertical Tabs on Firefox

It's also possible to get Edge-like vertical tabs on Firefox (If it's not apparent yet, I'm coming from Edge, and I still kinda like it). To get this feature, refer to [Firefox vertical tabs](https://github.com/ranmaru22/firefox-vertical-tabs) on GitHub. The repository contains all the instructions on how to enable this feature.

After setting up vertical tabs, there may be a weird spacing on the top-right. To get rid of that:

* Right-click anywhere on the Firefox toolbar and click on "Customize Toolbar"
* Turn on Title Bar on the lower-left. The weird spacing will now be gone.
