# My Firefox Setup

## Addons Install
- [Greasemonkey](https://addons.mozilla.org/de/firefox/addon/greasemonkey/)
- [HTTPS Everywhere](https://addons.mozilla.org/de/firefox/addon/https-everywhere/)
- [Startpage Private Search](https://addons.mozilla.org/de/firefox/addon/startpage-private-search/?src=search)
- [uBlockOrigin](https://addons.mozilla.org/de/firefox/addon/ublock-origin/)
- (*optional*) [uMatrix](https://addons.mozilla.org/de/firefox/addon/umatrix/?src=search)

### AntiAdblock Setup

#### [Anti-Adblock Defuser by Nano Defender](https://jspenguin2017.github.io/uBlockProtector/) installation for uBlock Origin

   1. Subscribe to [Adblock Warning Removal List](https%3A%2F%2Feasylist\-downloads.adblockplus.org%2Fantiadblockfilters.txt&amp;title=Adblock%20Warning%20Removal%20List) 
      
     ubo://subscribe?location=https%3A%2F%2Feasylist\-downloads.adblockplus.org%2Fantiadblockfilters.txt&amp;title=Adblock%20Warning%20Removal%20List
      
   2. Subscribe to [Nano Defender Integration filter list](https%3A%2F%2Fgitcdn.xyz%2Frepo%2FNanoAdblocker%2FNanoFilters%2Fmaster%2FNanoMirror%2FNanoDefender.txt&amp;title=Nano%20Defender%20Integration)
   
     ubo://subscribe?location=https%3A%2F%2Fgitcdn.xyz%2Frepo%2FNanoAdblocker%2FNanoFilters%2Fmaster%2FNanoMirror%2FNanoDefender.txt&amp;title=Nano%20Defender%20Integration
   
   3. Go to uBlock Origin dashboard, select `Settings` tab, check `I am an advanced user`, click the gears icon that shows up, replace `unset` after `userResourcesLocation` by:
        
   > https://<i></i>gitcdn.xyz/repo/NanoAdblocker/NanoFilters/master/NanoFilters/NanoResources.txt`
        
   **Warning:** The resources file is not a filter list, do not load it as a filter list or things will break
   
   4. Subscribe to [Nano Filters](https%3A%2F%2Fgitcdn.xyz%2Frepo%2FNanoAdblocker%2FNanoFilters%2Fmaster%2FNanoFilters%2FNanoBase.txt&amp;title=Nano%20filters)
   
     ubo://subscribe?location=https%3A%2F%2Fgitcdn.xyz%2Frepo%2FNanoAdblocker%2FNanoFilters%2Fmaster%2FNanoFilters%2FNanoBase.txt&amp;title=Nano%20filters`
        
#### [Anti-Adblock Killer](https://reek.github.io/anti-adblock-killer/) installation as *userscript* and filter list subscription

   1. Install script [Anti-Adblock Killer](https://raw.github.com/reek/anti-adblock-killer/master/anti-adblock-killer.user.js)
   2. Subscribe to [AakList (Anti-Adblock Killer)](https://raw.github.com/reek/anti-adblock-killer/master/anti-adblock-killer-filters.txt&amp;title=AakList )
   
    abp:subscribe?location=https://raw.github.com/reek/anti-adblock-killer/master/anti-adblock-killer-filters.txt&amp;title=AakList (Anti-Adblock Killer))

## Privacy Settings

   1. Go to `Settings`select `Privacy & Security` and set `activity tracking protection`to `user defined`change `tracking content`to always
   2. Set `Do Not Track` to always
   3. In the `Cookie` section, set the tick on `delete cookies if firefox is closed`and define exceptions

## Theming
   * Select "Arc Dark Theme" on Linux or "Windows 10 dark test" on Windows 
