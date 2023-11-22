# FIREFOX ABOUT:CONFIG TWEAKS

**Use Action Center notifications** <br/>
**Use system roots certification storage**
```
user_pref("alerts.useSystemBackend", true);
user_pref("security.enterprise_roots.enabled", true);
```

**"Edge like scrolling" experience**

```
user_pref("general.smoothScroll", true);
user_pref("general.smoothScroll.currentVelocityWeighting", "0.15");
user_pref("general.smoothScroll.mouseWheel.durationMaxMS", 250);
user_pref("general.smoothScroll.mouseWheel.durationMinMS", 250);
user_pref("general.smoothScroll.msdPhysics.enabled", true);
user_pref("general.smoothScroll.msdPhysics.motionBeginSpringConstant", 400);
user_pref("general.smoothScroll.msdPhysics.regularSpringConstant", 600);
user_pref("general.smoothScroll.msdPhysics.slowdownMinDeltaMS", 120);
user_pref("general.smoothScroll.other.durationMaxMS", 500);
user_pref("general.smoothScroll.pages.durationMaxMS", 350);
user_pref("general.smoothScroll.stopDecelerationWeighting", "0.8");
user_pref("mousewheel.min_line_scroll_amount", 22);
```

**Privacy, disabing Mozilla Telemetry and sponsor content**

```
user_pref("browser.newtabpage.activity-stream.feeds.discoverystreamfeed", false);
user_pref("browser.newtabpage.activity-stream.feeds.telemetry", false);
user_pref("browser.newtabpage.activity-stream.section.highlights.includePocket", false);
user_pref("browser.ping-centre.telemetry", false);
user_pref("browser.tabs.crashReporting.sendReport", false);
user_pref("extensions.pocket.enabled", false);
user_pref("services.sync.prefs.sync-seen.browser.newtabpage.activity-stream.feeds.section.topstories", false);
user_pref("services.sync.prefs.sync-seen.browser.newtabpage.activity-stream.showSearch", false);
user_pref("services.sync.prefs.sync-seen.browser.newtabpage.activity-stream.showSponsored", false);
user_pref("services.sync.prefs.sync-seen.browser.newtabpage.activity-stream.showSponsoredTopSites", false);
```

**Disable Firefox Account Login button and tab in settings**

If you don't using Firefox Account sync - hide buttons and options in settings. 
```
user_pref("identity.fxaccounts.enabled", false);
```

**Edge-FrFox theme tweaks for Windows 11 Mica like theme** <br/>
Copy `chrome` directory from `chrome.zip` file to your Firefox profile dir. See `about:support` page for details. <br/>
Sample PATH `%APPDATA%\Mozilla\Firefox\Profiles\abcd1234.default-release` <br/>
Add to `about:config` following tweaks (or edit `prefs.js` self)
```
user_pref("layout.css.color-mix.enabled", true);
user_pref("svg.context-properties.content.enabled", true);
user_pref("toolkit.legacyUserProfileCustomizations.stylesheets", true);
user_pref("uc.tweak.disable-drag-space", true);
user_pref("uc.tweak.floating-tabs", true);
user_pref("uc.tweak.floating-tabs.equal-margin", true);
user_pref("uc.tweak.force-tab-colour", true);
user_pref("uc.tweak.hide-newtab-logo", true);
user_pref("uc.tweak.remove-tab-separators", true);
user_pref("uc.tweak.rounded-corners", true);
user_pref("uc.tweak.show-tab-close-button-on-hover", true);
user_pref("uc.tweak.smaller-context-menu-text", true);
user_pref("uc.tweak.win11-mica", true);
user_pref("browser.tabs.tabClipWidth", 86);
user_pref("browser.tabs.tabMinWidth", 66);
```

Install Mica For Everyone and apply conf file setting also. 
Install `MSEdgeRedirect.exe` and redirect Microsoft Edge URLs to Firefox. 
Remove Edge via Remove-MS-Edge tool. Read README.md from zip before use.


# FIREFOX ADDONS

- https://addons.mozilla.org/firefox/addon/adguard-adblocker/
- https://addons.mozilla.org/firefox/addon/bitwarden-password-manager/
- https://addons.mozilla.org/firefox/addon/bookmarks-clean-up/
- https://addons.mozilla.org/firefox/addon/browser-cleaner-pro/
- https://addons.mozilla.org/firefox/addon/cookiebro/
- https://addons.mozilla.org/firefox/addon/enhancer-for-youtube/
- https://addons.mozilla.org/firefox/addon/fastforwardteam/
- https://addons.mozilla.org/firefox/addon/new-tab-speed-dial/
- https://addons.mozilla.org/firefox/addon/polish-cookie-consent/
- https://addons.mozilla.org/firefox/addon/search_by_image/
- https://addons.mozilla.org/firefox/addon/simple-translate/
- https://addons.mozilla.org/firefox/addon/sponsorblock/
- https://addons.mozilla.org/firefox/addon/to-google-translate/
- https://addons.mozilla.org/firefox/addon/tonec-idm-integration-module/
- https://addons.mozilla.org/firefox/addon/view-image/
- https://addons.mozilla.org/firefox/addon/violentmonkey/
- https://addons.mozilla.org/firefox/addon/wikiwand-wikipedia-modernized/
- https://github.com/AdguardTeam/AdGuardExtra

<hr/>

# CREDITS

- https://github.com/bmFtZQ/Edge-FrFox
- https://github.com/MicaForEveryone/MicaForEveryone
- https://github.com/rcmaehl/MSEdgeRedirect
- https://github.com/ShadowWhisperer/Remove-MS-Edge
