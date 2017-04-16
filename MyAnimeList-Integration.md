MyAnimeList Integration adds the ability to add and update your MAL  directly from 9anime. However, it adds very minimal information to you MAL. 
* **Add To MAL** adds the name of the anime, sets the status as watching and sets the started watching date to today.
* **Update MAL** only updates the Episode. 

*For more customization, please use MyAnimeList directly.*

# FAQ
### Where are my username and password stored?
**Your username and password are stored in Plain Text in chrome.local/browser.local storage. It is not transmitted anywhere else.** 
You can view the saved settings along with all the other settings by inspecting the `background.html`
![](https://preview.ibb.co/mU9vbQ/bg.png)

and using this code in the console:
```js
chrome.storage.local.get(function (saved) {
	console.log(saved);
})
```
### Does that mean my username and password are not safe?
Unless someone else physically inspects the storage or modify the extension, you are safe.

### Well that does not sound very convincing. Anything else that I can do?
Yup. You can verify your credentials when you are using the integration and remove your credentials when you are not. Oh and also since this is a open source project, feel free to verify the code as well 😄 