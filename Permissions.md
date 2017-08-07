9anime Companion needs extension permissions to function properly. Lets take a look at why they are necessary.

## Remove Ads
![Remove Ads Popup](https://image.ibb.co/noUvUv/rem_Ads_perms.png)

When you enable remove ads setting, you will probably see a popup like the one above. *Read and change all of your data on the websites you visit* sounds like a serious permission. But why do we need it just to remove Ads? What is happening is, it is asking for these permissions:

```json
{
        "origins": ["<all_urls>"],
        "permissions": [
            "webRequest",
            "webRequestBlocking"
        ]
    }
```
This part `"origins": ["<all_urls>"]` is responsible for showing that line. So why exactly does 9anime Companion need this? For that you need to understand how the remove ads work. It works in 3 parts.

#### Background Script (Most Important)
It matches url's of requests from a list of urls that are known ad provider/malicious and cancels them (so the request never happens). This is very much like how normal adblockers work. Since 9anime Companion needs to analyze all the request url's to cancel out the bad ones, the `"origins": ["<all_urls>"]` is required.

#### Global Content Script
Overwrites a few functions that generates popups making them useless

#### Watch Page Content Script
Removes ads from the watch page via selectors, and also clears up the ad placeholders.
