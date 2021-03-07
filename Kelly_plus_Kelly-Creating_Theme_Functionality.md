## [Creating Theme Functionality - Sept 30, 2020](https://www.youtube.com/watch?v=wR8L-0QnKZo&t=392s)

In this recording Kelly Vaughn and Thomas Kelly explore how to add functionality into your theme projects, and explore some of the features you can build in your theme.

The Kellys will walk you through how to:

- Create a custom section that displays a free shipping bar
- Display dynamic updates for cart properties
- Set up free shipping thresholds
- Apply styling to a custom section

--------------------------------
Subscribe to our channel for more videos about developing and designing ecommerce stores, apps, and themes with Shopify » www.youtube.com/shopifydevs​

Looking for more information about developing on Shopify check out www.developers.shopify.com and https://shopify.dev/​

Connect with us on Twitter » www.twitter.com/shopifydevs

Launch your own online store by visiting Shopify and starting your free trial » http://bit.ly/VisitShopify

* * *
<br>

Notes:
- Kelly Vaughn "you don't always need an app to solve some basic problems". Only takes a bit of coding and building a custom section, which can be used in future projects as well.
- Conversion rate optimization (CRO). Anything for CRO is great especially something like a free shipping bar that counts down when you are getting to that free shipping threshold
- imposter syndrome is a thing. it's ok to google, search, for something. shopify.dev site is also your friend. live by it as well.
- Section everywhere is still coming "Soon".
- Can tune into partner town hall webcast:
	- [October 2020 Partner Town Hall](https://www.youtube.com/watch?v=QGGhpiuKFGw)
	- [October 2020 Partner Town Hall - Asia-Pacific Countries (APAC)](https://www.youtube.com/watch?v=3j7mbZsypew)
- Make theme easy as possible for merchant to update site without breaking things
- sections "super important" to allow customization and to make sure you set up settings correctly
- Three different tags can include in a section
	- `{% schema %}{% endschema %}`
	- `{% stylesheet %}{% endstylesheet %}`
	- `{% javascript %}{% endjavascritp %}`

	![2021-02-16 19_52_35-{{ Kelly plus Kelly }} Creating Theme Functionality - Sept 30, 2020.mp4 - VLC me.png](:/f48588a1a97f42eb90e2abc63de6d051)
- Use `{% javascript %}{% endjavascritp %}` tags in section, when needed. having a master javascript file where section(s) pulling from loads unnecessary bits to your site.
- Always want to define section by defining it with a name, it's settings, class and/or presets.
	- [Required attributes for input settings](https://shopify.dev/docs/themes/settings#attributes-for-input-settings):
		- `type` - "Name of the type of settings".
		- `id` - uniqure name for this setting. "id is e[xposed to the Liquid templates](https://shopify.dev/tutorials/develop-theme-theme-editor-other-theme-files#access-settings-inputs) via the [settings](https://shopify.dev/docs/themes/liquid/reference/objects#settings) or [section.settings](https://shopify.dev/docs/themes/liquid/reference/objects/section#section-settings) objects".
		- `label` - "A label for this setting". A friendly readable field/area describing what the content `type` is to here for and/or will be doing.
	```json
	{
      "type": "text",
      "id": "free-shipping-threshold",
      "label": "Free Shipping Threshold",
      "info": "Include number only. Don't include the $."
    },
	```
	![1fd7ffcd33875e6e1d5667527df9776e.png](:/807195af300c493ab07d46e9154612fb)
- multiple `schema` types that can be used
- for `schema` > `settings` > content `type` we will use of "text" a lot.
- If a section is created and not called anywhere, e.g. theme.liquid, then it will not show up in theme style area. Created section needs to be called, or declared, somewhere first.
![621b1f9f2eeaa545e08f979c8238ad78.png](:/335e946828054625834f4f387de56b24)
- No local shopify development for shopify theming. For "local" development, we can use [webpack](https://webpack.js.org/) or [browsersync](https://www.browsersync.io/docs). those are the ones Thomas have used in past, he stated.
- I am pretty sure there are some other ones that can simulate local dev for shopify, might have to search into this some more.
- to get free shipping bar feature to work, we at least need to know subtotal, hence we are going to need to use the "cart" object: `cart.items_subtotal_price`
- "shopify" "object" and whatever object you are looking in google search will usually bring you to correct shopify page, e.g. "[shopify object cart](https://www.google.com/search?q=shopify+object+cart&oq=shopify+object+cart&aqs=chrome..69i64j0i22i30l2j69i57.8633j0j1&sourceid=chrome&ie=UTF-8)" or "[shopify cart object](https://www.google.com/search?newwindow=1&sxsrf=ALeKk00aiuWFZ-dJwZQ0pwSXCpSy0WWNgA%3A1613531791100&ei=j4osYKLMBbKl5NoP0NebcA&q=shopify+cart+object&oq=shopify+cart+object&gs_lcp=Cgdnd3Mtd2l6EAMyBAgAEEMyBggAEBYQHjoHCAAQRxCwA1DFxUlYxcVJYJ3PSWgBcAJ4AIABoQOIAcYEkgEHMC4xLjQtMZgBAKABAqABAaoBB2d3cy13aXrIAQjAAQE&sclient=gws-wiz&ved=0ahUKEwjiz_ep-u_uAhWyElkFHdDrBg4Q4dUDCA0&uact=5)"
- If I got this straight, `cart.items_subtotal_price` [doesn't do currency conversion](https://shopify.dev/docs/themes/liquid/reference/objects/cart). It gives you whole number, such as instead of $3.50, in the example in the video, we see 350. We need to use the `money` [object/filters](https://shopify.dev/docs/themes/liquid/reference/filters/money-filters) to do the conversion.
- Block `name` has a 25 character limit.
- Disabling cart notification. Notification works through javascript/cart.js route, which lets you ajax/fetch request to get cart current state without having to reload page. Without doing this we would have had to code shipping bar around that. So for this webinar {{ Kelly | plus: Kelly }}, it was disabled instead.
- [Money Filter](https://shopify.dev/docs/themes/liquid/reference/filters/money-filters) performs, as stated earlier, currency conversion, especially for localization purposes.
- When building the shipping bar feature, advise is to built-in the conversion within it by using the [money filter](https://shopify.dev/docs/themes/liquid/reference/filters/money-filters)
![af7b6d4afa9f7deb3c6ff5ed72c39f7c.png](:/d7ad0006dc0144b3bba6839b46dcde6f)
![42b3334da21b644d054690c2b9102c02.png](:/051ab8938e804cd4b7ffef03b8dcc430)
- To update shopify theme automaticaly from [vscode](https://code.visualstudio.com/), run `theme watch`. We can also setup a .js file and use npm to run the watch command as well. More on this in next video in {{ Kelly | plus: Kelly }} series!
- `Theme watch` is watching for any changing in the theme folder and as soon as something is changed, uploads changes automatically.
- `Theme watch` does not do live reloading. Handles changes. Once changes are uploaded to shopify, you have to refresh browser manually.
- Going back to earlier mention, [browsersync](https://www.browsersync.io/docs) and/or [webpack](https://webpack.js.org/) can be use to setup some sort of "live reload", locally. see respective options for more details.
- Setting up "shipping bar" message
![a416b4e87bc50bcfd27b99607b26481e.png](:/07f1086d2abf47b0b5339f1f3079c21a)
- When dealing with Ajax cart, you have to refresh page to see changes for you to see the changes made:
![8ee6ca3546f792386f3ce39bb9ddd5aa.png](:/d8451a85c3284fb2b43b43aa399db0ec)
![65806a737a49ccf32929a4580faf3500.png](:/e62e8676ac6340cdac5567484394ed33)
- Replacing `*` in the message with currency
![fe0670f66d2b867c4e8b2648c923e92c.png](:/ba1e8f7c75ae4c9b96f90144bf47de51)
![f9a97f709631034dc0503fd6f5e7c7de.png](:/00c42dc533d147b1918777059ef9fe87)
- To not have to reload page to see changes to shipping bar, we would need to setup javascript/fetch to get info we need without having to depend on Ajax reload.
- We would need to add javascript to cart coding to make this work.
- Adding styles to the "shipping bar" feature.
- Thomas went to Debut and looked to used the "announcement bar" style but since not enabled, decided to go ahead with setting up styles in section instead.
- Kelly also added the schema settings for a merchant to be able to make color changes to shipping bar.
![ca88581948c0bc5a23b2341af51c321e.png](:/b7cde2dfe2f64a75be8b929c8053743c)
- updating styles sections in "shinpping-bar" sections file
![7ecd6aa987c6f6337afac742d05f4abd.png](:/498ba2a6acc84935a643a9d7ca8e533b)
![666c7bd2013345a20201ea97d4d1d3f4.png](:/74e67d87492640ab86d446d5857b112b)
- Settings applied:
![931e5893725ef31a9a6faaf1c8c7dd75.png](:/eef7c8eeb8714a3aa02f558df50fc3e3)
![cc1ae2501867283a69a108e95908b8f8.png](:/b3ffce3062154093ad36d59801dd66dd)
- we ended up creating a "free-shipping-section" that has a "threshold" and is keeping track of what's remaining and will update until free shipping threshold is hit/achieved.
- Once the "threshold" is meant, then it will automatically change to correct message letting customer know they qualify for free shipping.
- We are not, however, using Ajax add a cart, as the Debut theme is using Ajax Add a cart.
- To make use of Ajax add a cart, we would add a `<span></span>` to the asteric's `*`, `<span>*</span>`, then use the Ajax add a cart function to look at the data attribute first for the free shipping threshold and then have it substract it from the cart subtotal and then render the new amount.
- Liquid syntax cannot be used in schema settings. One, because of when liquid renders. Two, because .json files will not like it, since it deals with "text".
- Thomas and Kelly are using Liquid extension by Nikos for liquid syntax highilighting.
![ccf5a59c2301e2fe1ac60021e36d7228.png](:/4f00e68c01e246fc8e27d12c9d8b94d7)
- Next episode will be "Theme Performance"


* * *

### Legend

[![a60a1e77ce0af253dfa441637cb357b6.png](:/0aac0d30dd5844bf8548473715131975)](https://twitter.com/kvlly)

- `{{ Kelly | }}` = [Kelly Vaughn](https://www.linkedin.com/in/kellyvaughn/)

[![4f9d4f51b887e1264249a8df7a595ba9.png](:/a0169c72c61a4ebcb0157841df70ba20)](https://twitter.com/thommaskelly)

- `{{ | plus: Kelly }}` = [Thomas Kelly](https://github.com/t-kelly)

* * *

### Links
- Content schema - List of content types: https://shopify.dev/docs/themes/sections/content-schema#list-of-content-types
- kellyvaughn-shipping-bar.liquid: https://gist.github.com/kellyvaughn/a4c02c27863582c760f20894093db45e
- https://gridsome.org/plugins/gridsome-source-shopify
- https://github.com/github/renaming
- https://ohzsh.sh
- https://shopify.dev/docs/themes/settings
- Browser Sync:
	- https://www.npmjs.com/package/browsersync-themekit
	- https://www.browsersync.io/docs

<br>
