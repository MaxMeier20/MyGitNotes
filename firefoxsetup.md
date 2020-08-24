# My Firefox Setup

## Addons Install
- [Greasemonkey](https://addons.mozilla.org/de/firefox/addon/greasemonkey/)
- [HTTPS Everywhere](https://addons.mozilla.org/de/firefox/addon/https-everywhere/)
- [I don't care about cookies](https://addons.mozilla.org/de/firefox/addon/i-dont-care-about-cookies/)
- [Startpage Private Search](https://addons.mozilla.org/de/firefox/addon/startpage-private-search/?src=search)
- [uBlockOrigin](https://addons.mozilla.org/de/firefox/addon/ublock-origin/)
- (*optional*) [uMatrix](https://addons.mozilla.org/de/firefox/addon/umatrix/?src=search)*

\* *The uMatrix extension is powerful but needs to be adapted for many sites to display correctly - This only makes sense on daily driver machines, that are extensively used

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
   * Set `Do Not Track` to `Always`
   * In the `Cookie` section, set the tick on `Delete cookies if firefox is closed`and define exceptions
   2. Go to `Settings` open the `General`section 
   * Allow DRM
   * (*optional*) Scroll all the way dow, open `Connection Settings` and (de-)select `DNS-Over-HTTPS` (deselect for private networks / select for networks controlled by others)

## Theming
   * Select "Arc Dark Theme" on Linux ( on Windows 10, the "Standard" theme should reflect the OS theming: if not "Windows 10 dark test" is available) 

# My Opera Setup

## Video Playback Issue

As Opera doesn't play .h264 video, the problem is easily solved by replacing `/usr/lib/x86_64-linux-gnu/opera/libffmpeg.so `with a fully licensed version of the library - either included in Google Chrome / Chromium and in many commmercial games from steam
