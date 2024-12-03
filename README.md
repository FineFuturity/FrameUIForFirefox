# Codename: FrameUI For Firefox
A new way to view your web content, like looking at photos printed from an old Polaroid camera.

![a1fd4499dd2be9a2ecccc660a6ce0696](https://github.com/FineFuturity/FrameUIForFirefox/assets/19298107/75c5a475-d440-4481-a002-9cdb754155ed)

# Changelog
**Version 0.3c:**
* issues noted for fixing in the 0.3b release notes have been fixed.
* the new sidebar introduced in the most recent update broke third-party vertical tab compatibility and the auto-hover css code.  functionality has been restored and vertical tab extensions should work again.
  * native vertical tab support was introduced in the latest firefox update, which is baked into the new sidebar when you enable it in about:config.  Compatbility with native vertical tabs will come in a future update. 

**Version 0.3b:**
* 12/2/2024 emergency release - The recently released Firefox update caused all toolbar elements to disappear, causing FrameUI to become unusable.  This emergency release restores core functionality while I work on fixing the lingering issues below for the next update.
* Lingering issues:
 * The private browsing icon was shifted left and associated label came back.
 * The menu bar is no longer underneath the address bar.  
  
**Version 0.3a:**
* The latest Firefox update caused some issues with clicking on interface elements, including the window controls.  The latest update to the theme fixes this issue.
  * I'm not sure if the update caused any other issues, so please report them as you see them.  
* Fixed the alignment of the private browsing indicator when in private browsing mode.
 

**Version 0.3:**
* Better support for configurations where the title bar buttons are either on the left or right side of the window, regardless of OS.
  * HUGE thanks to MrOtherGuy's CSS ![code](https://github.com/MrOtherGuy/firefox-csshacks/blob/master/chrome/toolbars_below_content.css), without which I would not have been able to fix this as well as the below issues.
* Fixed issues with the menubar not playing nicely with the navigation bar when it's active.
* Fixed issue with the private browsing indicator icon being misaligned with the navigation bar when in private browsing mode.
* Fixed issue where the bookmarks toolbar would push the navigation toolbar past the bottom window boundary if "Only Show on New Tab" was set.
* When clicked, the address bar's URL text now stays at the bottom rather than moving to the top.
  * This should make typing a URL or search term much less jarring.


**Version 0.2:**
* Initial macOS support.
  * Platform detection has been added, so the theme now accounts for configurations where either the title bar buttons are on the left (e.g., macOS/Linux title bar buttons on left) or on the right (e.g, Windows/Linux title bar buttons on right).
* Fixed issue with user-selected themes either working inconsistently or not at all.
* Inactive window title bars are now darker to differentiate them from the active window.
 
**Version 0.1:**
* Initial release

# Known Issues
* The entire area of the nav bar cannot be used to drag the window in the 0.3 update.
  * I am still figuring out how MrOtherGuy's code works and should be able to fix this in the next update.

* ~~Haven't found any just yet.  Please report if you find any. :)~~
* ~~Menu bar overlaps with the navigation bar when it's active.~~
* ~~The private browsing indicator icon is misaligned with the navigation bar when in private browsing mode.* The bookmarks toolbar pushes the navigation toolbar past the bottom window boundary if "Only Show on New Tab" was set.~~
* ~~When clicked, the address bar's URL text moves to the top of the results dropdown rather than staying in place.~~



**macOS NOTE:**
* FrameUI was designed to have the window control buttons on the bottom. However, due to the way that fullscreen windows work on macOS, the window control buttons will remain at the top of the window like other macOS apps. This complication is not present in windowed mode.

# Screenshots
![image](https://github.com/FineFuturity/FrameUIForFirefox/assets/19298107/73b7328d-3b6c-47f6-b4fe-d341aa46b88b)
![image](https://github.com/FineFuturity/FrameUIForFirefox/assets/19298107/ed6123fd-b6fd-4124-b264-a83468fa1bc8)
![image](https://github.com/FineFuturity/FrameUIForFirefox/assets/19298107/3b7a9f63-6cae-43de-bfb0-d07fd28b8d10)
![image](https://github.com/FineFuturity/FrameUIForFirefox/assets/19298107/f64bbb3e-217e-4f78-a9fe-da2ebeb3b265)



<h4>Now with theme support!</h4>

![image](https://github.com/FineFuturity/FrameUIForFirefox/assets/19298107/17ade781-524a-49e5-99d7-c8b72ceb131a)
![image](https://github.com/FineFuturity/FrameUIForFirefox/assets/19298107/3dba5c46-b83f-4877-b289-67b5aa9949c0)
![image](https://github.com/FineFuturity/FrameUIForFirefox/assets/19298107/2beeeb4b-99d6-4316-87cf-ca461f959516)



# Prerequisites
* For this to work, make sure `toolkit.legacyUserProfileCustomizations.stylesheets` is set to `true` in `about:config`.
* To make the most of this theme, it is **STRONGLY recommended** that you install an addon for vertical tabs, such as Tab Center Reborn.  **This is a stopgap for now until I figure out how to integrate native vertical tab functionality into the theme.**
* If you're on Linux, make sure your window controls are set to be on the right side of your title bar.

# Installation

Simply drop the provided `userChrome.css` file into your `chrome` folder and restart for the changes to take effect.

# Motivation
After restarting, you'll notice that *all* of the controls -- the navigation bar, the window controls, *everything* -- has been moved to the bottom in a manner reminiscent of the Metro-based Internet Explorer app seen in Windows 8/8.1.  While I think Microsoft was on the right track with their attempts at a tablet-based interface... well, we all know what happened.  Apart from Microsoft's attempt at a touch interface (which was a half-done attempt anyway), I think no company to this day has yet to get right.

This theme is a step towards what I believe may solve the grand problem of unifying the desktop and tablet interface for ANY device form factor.  What I hope you'll find is that this interface works really well on *both* tablet and desktop form factors, precisely because there is no longer a need for a user to lift their arms to get to something as basic as the window controls -- they're now just a mere finger reach away.  

# Reporting Issues
FYI, this project is my first go at using CSS.  As this is the initial release on top of that, I anticipate there will be issues.  If you encounter any bugs or other issues, please post a thread and I'll do what I can, when I can. 

Also: as this theme is a both a thought experiment and work in progress, it is possible the look and feel will change over time.  I welcome any and all suggestions for how this could be improved.  :)

# Credits
* HUGE SHOUTOUT to MrOtherGuy's ![Collection of random CSS hacks for Firefox](https://github.com/MrOtherGuy/firefox-csshacks) repo.
* Private testers (who I can name here if they wish)

