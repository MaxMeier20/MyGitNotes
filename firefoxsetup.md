# My Firefox Setup

## Addons
- Greasemonkey
- HTTPS Everywhere
- Startpage.com
- uBlockOrigin
- (*optional*) uMatrix

### AntiAdblock Setup

#### [Anti-Adblock Defuser by Nano Defender](https://jspenguin2017.github.io/uBlockProtector/) installation for uBlock Origin

        <p>Step 1. Subscribe to <a href="ubo://subscribe?location=https%3A%2F%2Feasylist-downloads.adblockplus.org%2Fantiadblockfilters.txt&amp;title=Adblock%20Warning%20Removal%20List">Adblock Warning Removal List</a>.</p>
        <p>Step 2. Subscribe to <a href="ubo://subscribe?location=https%3A%2F%2Fgitcdn.xyz%2Frepo%2FNanoAdblocker%2FNanoFilters%2Fmaster%2FNanoMirror%2FNanoDefender.txt&amp;title=Nano%20Defender%20Integration">Nano Defender Integration</a> filter list.</p>
        <p>Step 3. Go to uBlock Origin dashboard, select <code>Settings</code> tab, check <code>I am an advanced user</code>, click the gears icon that shows up, replace <code>unset</code> after <code>userResourcesLocation</code> by:</p>
        
        <p><code>https://gitcdn.xyz/repo/NanoAdblocker/NanoFilters/master/NanoFilters/NanoResources.txt</code></p></div>
        
        <p><strong>Warning:</strong> The resources file is not a filter list, do not load it as a filter list or things will break.</p>
        <p>Step 4. Subscribe to <a href="ubo://subscribe?location=https%3A%2F%2Fgitcdn.xyz%2Frepo%2FNanoAdblocker%2FNanoFilters%2Fmaster%2FNanoFilters%2FNanoBase.txt&amp;title=Nano%20filters">Nano filters</a>.</p>
        
#### [Anti-Adblock Killer](https://reek.github.io/anti-adblock-killer/) installation as *userscript* and filter list subscription

    1. Install script [Anti-Adblock Killer](https://raw.github.com/reek/anti-adblock-killer/master/anti-adblock-killer.user.js)
    2. Subscribe to [AakList (Anti-Adblock Killer)](abp:subscribe?location=https://raw.github.com/reek/anti-adblock-killer/master/anti-adblock-killer-filters.txt&amp;title=AakList \(Anti-Adblock Killer\))

