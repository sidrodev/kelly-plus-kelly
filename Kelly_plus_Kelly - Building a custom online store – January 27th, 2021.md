## [{{ Kelly | plus: Kelly }} Building a custom online store – January 27th, 2021](https://youtu.be/wcIYoOsjxdE)

A new year brings new beginnings! Join Kelly Vaughn and Thomas Kelly as they get started building out their custom Shopify online store. Follow the build LIVE every Wednesday @2PM EST at <https://twitch.tv/shopifydevs>​. Code available at <https://github.com/t-kelly/shopipoint>...​

Mentioned Links:

- Rapidly build modern websites without ever leaving your HTML: <https://tailwindcss.com/>​
- Load optimized npm packages with no install and no build tools: <https://www.skypack.dev/>​
- Frontend build tool: <https://www.snowpack.dev/>​
- Multipass: <https://shopify.dev/docs/admin-api/rest/reference/plus/multipass>
- Multipassify - Shopify Multipass module for Node.js: <https://github.com/beaucoo/multipassify>​
- Build a Shopify App with Node and React: <https://shopify.dev/tutorials/build-a-shopify-app-with-node-and-react>
- Branding and Design Made Easy - Ready-to-use templates: <https://placeit.net>​
- Theme Check - Think RuboCop, or eslint, but for Shopify themes: <https://marketplace.visualstudio.com/items?itemName=Shopify.theme-check-vscode>
  - Theme Check -Think RuboCop, or eslint, but for Shopify themes: <https://github.com/Shopify/theme-check>​
- The routes object: <https://shopify.dev/docs/themes/liquid/reference/objects/routes>
- Get/Use kitten images as placeholders: <https://placekitten.com>​

----

Subscribe to our channel for more videos about developing and designing ecommerce stores, apps, and themes with Shopify » www.youtube.com/shopifydevs​

Looking for more information about developing on Shopify check out www.developers.shopify.com and <https://shopify.dev/>​

Connect with us on Twitter » www.twitter.com/shopifydevs

Launch your own online store by visiting Shopify and starting your free trial » <http://bit.ly/VisitShopify>

----

## Notes

- `{{ | plus: Kelly }}`: "One of the topics for today, that we going to speak on is [Theme Check](https://github.com/Shopify/theme-check). [Marc Cournoyer](https://github.com/macournoyer) has been working on this. It's something that, I think, we need to really pump up. This is huge! I'm so excited to see this out and already what it can do but the potential of what it can do too."
- `{{ Kelly | }}`: "Do you want to also talk about what our plans are for for the stream moving forward."
- `{{ | plus: Kelly }}`: "Yeah. So, what we talked about on how we want to approach this stream. Ultimately I'd say we were having trouble figuring out like what should we spend an hour talking about this topic? what should we talk about ahead of time? I think we both like the idea of just being able to approach this as "hey we want to spend an hour a week building out themes or actually building out an online store more than themes, building out an online store experience on shopify". Anything goes so that's what we're gonna do and it gives us and you guys the freedom to come here ask any questions you want, really steer the direction of what we might be working on. it gives us the freedom to just arrive and be "okay so what do we have to do to make this store working better?" So that is the start of it. The next part is what we've been working on? We've been working on this [repo](https://github.com/t-kelly/shopipoints.com) for a month or so now and it's been the subject of just some PRs that we've opened and that [repo](https://github.com/t-kelly/shopipoints.com) and that repo I'm talking about is [shopipoints.com](https://shopipoints.com/). Waht we want to do is build this online store experience, out in the public, and that experience is around the idea of [shopipoints.com](https://shopipoints.com/), we want to have a point system for the community. For you guys that are watching. What I was able to find, first of all, is that [Twitch](https://www.twitch.tv/shopifydevs) has a really cool [Twitch channel points](https://help.twitch.tv/s/article/channel-points-guide?language=en_US)."
- **Question**: Like store credit?
  - `{{ Kelly | }}`: "In a sense yes."
  - `{{ | plus: Kelly }}`: "Yes, yes. We want to get there. What [Twitch](https://www.twitch.tv/shopifydevs) already has setup, by the way I'm going to say that this is one way that you're going to be able to get [Shopipoints](https://shopipoints.com), is that [Twitch Channel Points](https://help.twitch.tv/s/article/channel-points-guide?language=en_US) rewards viewers for participating in the [Twitch](https://www.twitch.tv/shopifydevs). So you get points just for [watching this stream](https://www.twitch.tv/videos/890448932). You get more points for repeat watches, like voting on polls, which I will promise to start a poll at some point in time. We'll have polls and we'll have more interactivity 😁 All this to say it's gonna be one way of getting [Shopipoints](https://shopipoints.com). So, what we're going to do is that we're gonna be working with the [Twitch API](https://dev.twitch.tv/docs/api/) to pull the viewers of our channel and their points that they have accumulated, into our [online store](https://shopipoints.com).  We're gonna have to figure out a way to use that information and use the [reward redeem feature on twitch](https://dev.twitch.tv/docs/api/reference#get-custom-reward-redemption), as well to translate that to a discount code or something. How do we translate channel points [Twitch channel points](https://help.twitch.tv/s/article/channel-points-guide?language=en_US)/[Shopipoints](https://shopipoints.com) into stuff that you can get/redeem on [shopipoints.com](https://shopipoints.com)."
- `{{ | plus: Kelly }}`: "And kelly i might ask you, so what types of things should we have on [shoppingpoints.com](https://shopipoints.com) because well you've got a store too. So what's your most popular merch?"
- At the time of this webcast, `{{ Kelly | }}` did have a store. To borrow her words, "to consolidate the number of projects I actively have running, something must go. Unfortunately the store was the unlucky winner..." She was looking to sell the assets, as "there have been some interest in purchasing the [assets of the business](https://shopkvlly.com/password)", however this offer was up to the 1st of March 2021, Monday this week.
![aae49e0fe1c3199d5db7e9870ed76d7d.png](:/11fb4ea7cc664e1e9dd4335965eface8)
- `{{ Kelly | }}`: "most popular merch?! I have a few things that I sell that are very popular. Mousepads, for one thing, I was not expecting mousepads to be so popular but they are. So, I have [Git Cheat Sheets](https://education.github.com/git-cheat-sheet-education.pdf) and [Regex Cheat Sheet](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions/Cheatsheet) mousepads and people really like them. Mugs are really popular. One of my best sellers is the `Git log` mug, which is a really sad story of me struggling on a project in the form of `Git log`. It contains a lot of things like "Please work" and "Help" and a lot of cursing , the usual developer process :laughing:"
- `{{ | plus: Kelly }}`: "So maybe like a theme-check/theme Linter mug?! Just playing off of your most popular items. Let's make this!"
- `{{ Kelly | }}`: "Could do a Liquid Cheat Sheet mug as well. That can be an option. We can make a bunch of Shopify jokes, somehow?! Ooh! let's do Section Everywhere Jokes :laughing:"
- `{{ | plus: Kelly }}`: "So, we'll have things that you'll be able to redeem [shopipoints](https://shopipoints.com) for. We have to set the price, but will figure that out later. So we're going to have the the online store portion of it that you're redeeming points, you have a leader board so people can also accumulate their points, especially once we start getting multiple sources for points not just the twitch channel. I'd really like to use any other APIs that kind of revolves around the [Shopify Community](https://community.shopify.com/c/Shopify-Community/ct-p/en)."
- `{{ Kelly | }}`: "Any kind of like loyalty program or something we can utilize their API."
- `{{ | plus: Kelly }}`: "Have a leader board of sorts and it's a Hub for this stream as well. So it will post the episodes of past streams and we can provide all the useful information. I really like how Jason's stream is setup"
- `{{ Kelly | }}`: "Learning with Jason"
- `{{ | plus: Kelly }}`: "Yes, [Learning with Jason](https://www.youtube.com/playlist?list=PLz8Iz-Fnk_eTpvd49Sa77NiF8Uqq5Iykx). I like how he posts transcripts of the streams. We can make our streams available there, on [shopipoints.com](https://shopipoints.com). A lot of the additional functionality that we're talking about, such as communicating with Twitch, is going to happen inside an app. So we will be building out a custom app for this store. Probably using app proxy, [Metafields](https://www.shopify.com/partners/blog/110057030-using-metafields-in-your-shopify-theme) API I imagine. We'll just store everything in [Metafields](https://www.shopify.com/partners/blog/110057030-using-metafields-in-your-shopify-theme), as it is a great way to kind of transfer data from an app to a store."
- `{{ Kelly | }}`: "I'm going to claim now that I want to build a Node app with [Koa](https://koajs.com/). We're going to have some middleware functionality, making sure that we keep a points balance. So, depending on what that looks like, I mean we could really just drive it through [loyaltylion](https://apps.shopify.com/loyaltylion) in that case. [Loyaltylion](https://apps.shopify.com/loyaltylion) was one of the many rewards options that would automatically deduct points for us so we would have that available, but then if we do a leader board, we probably don't  want to use the actual usernames of people so we could use something like  [Helium's Customer Fields App](https://apps.shopify.com/customr?surface_detail=helium&surface_inter_position=1&surface_intra_position=5&surface_type=search) to add some additional like add a username that gets added as a meta field and use that as the identity for each person."
- `{{ | plus: Kelly }}`: "Okay and is that linking to like the customers account?"
- `{{ Kelly | }}`: "Yes"
- `{{ | plus: Kelly }}`: "That was another part that we'll have to have people be able to log in to our store and then link their Twitch account so that we know that these points belong to you when you get to the checkout. I was just gonna say we'll have to talk about that but we'll have to talk about that on the stream because the whole point of this is that everything that we're working on here is going to be live streamed. We're really going to try not to do work on the side or research on the side and hopefully by committing to once a week that's okay, another big announcement, we're going to be doing this once a week, that we get some progress done. Now, no guarantees to how polished things will be. It's going to take time"
- `{{ Kelly | }}`: "we do have full-time jobs too! :laughing: :laughing:"
- `{{ | plus: Kelly }}`: "Maybe there will be some PR cleanups. Who knows! :laughing: :laughing:. I want to know what you guys want to see!"
- `{{ Kelly | }}`: "If you do have some ideas, definitely drop them in the chat. Question in the chat: 'Would it require [Multipass](https://shopify.dev/docs/admin-api/rest/reference/plus/multipass)?'" Answer: "This is not going to be a [Shopify Plus Store](https://help.shopify.com/en/manual/intro-to-shopify/pricing-plans/shopify-plus), so we won't have access to [Multipass](https://shopify.dev/docs/admin-api/rest/reference/plus/multipass). I assume you're not pulling you know secret [shopify plus](https://www.shopify.com/plus/platform) things."
- `{{ | plus: Kelly }}`: "I'm not aware of [Multipass](https://shopify.dev/docs/admin-api/rest/reference/plus/multipass) can you describe that?"
- `{{ Kelly | }}`: " so [Multipass](https://shopify.dev/docs/admin-api/rest/reference/plus/multipass) is a [Shopify Plus](https://www.shopify.com/plus/platform) feature where it allows you to log in with a third-party system so let's say you have a full user system like a forum for example and you want to add a store you already have all the logins set up on the forum so you basically use [Multipass](https://shopify.dev/docs/admin-api/rest/reference/plus/multipass) to log in on the forum it sends the data back to shopify it creates a customer record if one doesn't exist using their email address and then they never have to set like a  password on shopify they always use their forum login."
- `{{ | plus: Kelly }}`: "Wow! Okay, I'm going to have to dig into that."
- `{{ Kelly | }}`: "You do need to dig into it. We're using it for a project right now and it's a lot but it's a really powerful feature."
- `{{ | plus: Kelly }}`: "Does it does it run off of shopify accounts, the accounts.shopify.com IDs?"
- `{{ | plus: Kelly }}`: "Yeah. So, it has a unique login URL. It'd be something like "website.com/account/login/multipass" and that is what's used to actually pass back through to [Shopify](https://www.shopify.com/)."
- `{{ | plus: Kelly }}`: "Okay. We'll see. I am going to live that up to you `{{ Kelly | }}`. I could look into making that happen."
- `{{ Kelly | }}`: "You probably could, but not everybody here would probably have access to Shopify Plus. I am adding the link to the multi-pass documentation if you're curious, to kind of parse through it and see exactly how it works. You can use your favorite programming language to actually connect it, so it will not come as any surprise that we're using node for our connection and also actually I don't think it's actually built by shopify. It's actually an npm package called [multipassify](https://github.com/beaucoo/multipassify)."
- `{{ | plus: Kelly }}`: "Today I learned something new. I'm going to take a look after the stream too. So I like that idea, what you described for the custom App node.js with koa that's included in the scaffolding for the [Shopify App CLI](https://github.com/Shopify/shopify-app-cli) right?"
- `{{ Kelly | }}`: "It is, yes."
- `{{ | plus: Kelly }}`: " we'll be able to show off the shopify app cli."
- `{{ Kelly | }}`: "There's also a full shopify tutorial on shopify.dev on how to build a shopify app with node and react, so react powering the front end. I don't think we really need to worry about that right now, at some point, thought, it would be actually cool to show how we use that so we can have like an internal leader board, for example, or keeping track of how often people are redeeming points so we can bring in a react friend and use shopify polaris, the design system, to pull in some of those pieces."
- `{{ | plus: Kelly }}`: "Or i was thinking for the episodes list, we'll probably be pulling from [YouTube's API](https://developers.google.com/youtube/v3) to pull in the latest episodes and then we'll want to maybe add some additional stuff or we'll want to manage that listing of episodes, previous episodes?! There's opportunity for some internal [Shopify Admin Interface](https://help.shopify.com/en/manual/shopify-admin) there?!"
- `{{ Kelly | }}`: "Yes."
- `{{ | plus: Kelly }}`: "On another note, on the Theme side, the building side, [tailwindcss](https://tailwindcss.com/) seems to be a pretty popular CSS library. Some are saying "is this the next bootstrap?" I don't know."
- `{{ Kelly | }}`: "I don't want anything to be the next [Bootstrap](https://getbootstrap.com/)."
- `{{ | plus: Kelly }}`: " Maybe they're saying it in terms of popularity. If they are saying in that context, fine."
- `{{ Kelly | }}`: "If you are not familiar with TailwindCSS though, it is a CSS framework that is built to really speed up your development. In the development community, we are seeing more and more people pick it up. Also, I came across, I believe it was on product hunt, somebody's theme scaffolding that is built with it, where it automatically incorporates [Tailwind](https://tailwindcss.com/)as a framework to build on top of, pretty cool."
- `{{ | plus: Kelly }}`: "I like the look of Tailwind. It's something I want to get my hands dirty with it. Have you had a chance of getting your hands dirty with it?"
- `{{ Kelly | }}`: "I haven't, I would definitely be interested in getting my hands dirty with it."
- `{{ | plus: Kelly }}`: "What I really like about it is it's a common language that then can be configured like you can configure it with a config file. I'm thinking of Themes. Themes come with presets and if you could define that preset, as if that config file could be your theme settings?! There's some stuff I want to explore there. What this approach to [tailwindcss](https://tailwindcss.com/) looks like on the shopify platform. Ultimately, the final production version of your Stylesheets are built out and it's based on a config and I am thinking that config is almost similar to Theme Editor or Theme Settings. And, it then parses your HTML and will scrape out and "tree shake", get rid of any extra css."
- `{{ Kelly | }}`: "If you go on the [Tailwind](https://tailwindcss.com/)docs, on the left side under customization, you can take a look at how that configuration file works."
- `{{ | plus: Kelly }}`: "Ok, yeah!!! There is that and there is the way of including [tailwindcss](https://tailwindcss.com/). Yeah!!! This is what I was reading the other day. There's this whole built process with Tailwind. What if that built process leaved on our app and was served via an app proxy? So that whenever you make changes to, as you're developing your theme, you don't have any built tools locally on your theme. That you just work with these raw [tailwindcss](https://tailwindcss.com/) files and come time that you want to preview it, your app will fetch those raw [tailwindcss](https://tailwindcss.com/) files, build them On-Demand and then serve up that fully compiled... it even will have Assets API access and so it can even view your page, scrape out any extra CSS. I have this feeling that we could do something really cool with On-Demand CSS building."
- `{{ Kelly | }}`: "I think this is definitely something that we should dig into!"
- `{{ | plus: Kelly }}`: "Similar note is [Skypack](https://www.skypack.dev/). This is something I have been looking into over Christmas. Have you heard of [Skypack](https://www.skypack.dev/) before?"
- `{{ Kelly | }}`: "I have not."
- `{{ | plus: Kelly }}`: "So, this has been circulating inside of Shopify. So this idea Skypack is an On-Demand JavaScript bundling service that instead of bundling locally on your Dev machine, you can request a file and that file can have imports from other libraries. When you request that file, it's going to request all of its dependencies and bundle it up and serve it for you fully compiled, ready to go. Again, it's no build tools that live on your device, on your computer, all of that is offloaded and optimized on this service."
- `{{ Kelly | }}`: "Interesting. I have to completely change the way I think through our build process by using these kind of things."
- `{{ | plus: Kelly }}`: "That's it. I have been going down this rabbit hole over the past month. There's a shift happening in the web development community where people are starting to realize all these local build tools and all this configuration is just resulting in a really heavy developer experience, that has all these different parts of it that you have to download, set up and run. So, what is this way of kind of relying on web native functionality? How can we offload all this complexity to the service and just focus on regular bear files? Ideally little to no build process as possible."
- `{{ Kelly | }}`: "It would make it so easy to onboard new developers or third-party devs who happen to build on top of things as well, just because we have to integrate any third-party developer from another agency or freelancer coming in, they have to use our build process or else things get overwritten and don't follow our process. Yeah, there's just a lot that happens with it."
- `{{ | plus: Kelly }}`: "On that note, it makes things simpler. So, if you look at our [shopipoints.com](https://shopipoints.com) folder, ideally our theme is just the theme files. We don't have a source folder and we don't have a dist folder. We don't have a nodes module folder, maybe we won't even need one? Maybe we don't even need to run npm install?"
- `{{ Kelly | }}`: "What does that look like?"
- `{{ | plus: Kelly }}`: "Right! What would this development environment look like where you literally just `git clone` onto your machine and you have [`theme kit`](https://shopify.dev/tools/theme-kit) or some really light, global `CLI` installed that you're just syncing files, essentially, and you open it up and it works. So, this is a gut feeling!"
- `{{ Kelly | }}`: "This sounds to good to be true."
- `{{ | plus: Kelly }}`: "Let me look at the comments. David is saying 'my only concern with using [tailwind](https://tailwindcss.com/) for theme development is that we need to wait for liquid files to upload before seeing our changes, whereas with typical css, sass post css, we can use hot module replacement and see results instantly. I'm keen to actually give [tailwind](https://tailwindcss.com/) a go in full build though, it might change my mind.' So David seems interested to see. Cool. So the other half of [Skypack](https://www.skypack.dev/) is [snowpack](https://www.snowpack.dev/), which is kind of the local dev.
- `{{ Kelly | }}`: "Though it would be awesome, I would not trust it. That's how I feel. I'm skeptical. It's like I said, sounds to good to be true."
- `{{ | plus: Kelly }}`: "yea 😬. It's a feeling. It's a feeling at this point. This is the stuff I want to dig into though, on this stream. What's new? what's experimental? And that's why I might have to do some some digging outside of the stream but at least I'm gonna try to come back here and share and collect feedback and and get people's thoughts on does this work? does this not work? So stay tuned for stuff like that too. This will all pique your interest. I am going to say this, this is targeted towards, maybe, some of the more advanced developers that are looking for or to be involved in some of these conversations. So we're going to have that mixed in. I mean we're building this store from scratch.
- `{{ Kelly | }}`: "Literally building this store. Exactly."
- `{{ | plus: Kelly }}`: "Should we start building this store?"
- `{{ Kelly | }}`: "Let's start building the store."
- `{{ | plus: Kelly }}`:"Don't know if people..."
- `{{ Kelly | }}`: "It looks really good! :laughing:"
- `{{ | plus: Kelly }}`: :laughing: "Our store is really fast!!!"
- `{{ Kelly | }}`: :laughing: "It is so fast!!!" <!--- There is nothing in the store yet!! Hence the speed of it!!! :laughing: -->
- `{{ | plus: Kelly }}`: "Really fast!!!" :laughing:
- `{{ Kelly | }}`: Really proud of it! :laughing:"
- `{{ | plus: Kelly }}`: "With our lowercase 'cart'. So.."
- `{{ Kelly | }}`: "Question: 'Are you guys going to use Product Metadata?'"
- `{{ | plus: Kelly }}`: "Not sure which Metadata we are going to be using. I know we want to be using metadata for episodes and stuff like that but that wouldn't be product metadata?! That would be collections, maybe?!"
- `{{ Kelly | }}`: "Episodes are like blog articles."
- `{{ | plus: Kelly }}`: "Blog, yeah. That's true. Each one can be a post"
- `{{ Kelly | }}`: "We might find some use, for example we could utilize, let's say, once you hit a certain threshold in points. Let's say you score 10,000 [shopipoints](https://shopipoints.com), you are now a VIP or you're a platinum, or whatever you may want to call it, then you get access to new swag or new products that you didn't have access to before. We can use product tags and customer tag to allow you to see what you're able to buy if there's something extra or redeem, not buy.
- `{{ | plus: Kelly }}`: "You know my mind goes to 'what is this VIP emblem look like?'"
- `{{ | plus: Kelly }}`: ":laughing: We need a [shopipoints](https://shopipoints.com). What does a [shopipoints](https://shopipoints.com) looks like?! :laughing:
- `{{ Kelly | }}`: "I have a question?! What is our sighting going to look like?"
- `{{ | plus: Kelly }}`: "I want to say we're working on it :laughing:
- `{{ Kelly | }}`: "I want to say I am not a designer. I cannot draw anything. I don't design."
- `{{ | plus: Kelly }}`: "I started my career as a designer but since joining Shopify, I have been exclusively a developer. After seeing what designers do at Shopify, don't consider myself at all a designer. How much of the craft they take to the next level than I ever have!... Oh, we'll see. We want to be starting with HTML and then CSS, well we'll be starting with [Liquid](https://www.shopify.com/partners/blog/115244038-an-overview-of-liquid-shopifys-templating-language), ultimately first. We want to get the structure of everything out, and maybe that's where we can start. I mean we can layer on the design, you know. It can be a prototype. We'll do a rough version, live. Maybe, if anyone's watching that feels confident in their design chops, we can get some iterative feedback as we go, 'come on line height there'"
- `{{ Kelly | }}`: "We don't have a hero image... If we are generating product designs, ourselves, we can go through [printful](https://apps.shopify.com/printful), for example. For fulfillment we can use a service called [placeit.net](https://placeit.net/) to generate images that we can use. So, you can upload your design and then it's placed on top of videos or on top of images, for instance if your selling a mug, you can have somebody holding a mug with your image on it or something like that. We can use this to generate a hero image or a hero video, if we wanted to do that, all kinds of fun stuff... There is a question: 'with that - shameless plug: any openings at Shopify? (final year student, learning Shopify for over a year, have a open source GitHub action for Shopify)' Visit [shopify.com/careers](https://www.shopify.com/careers). Since I don't work for [Shopify](https://www.shopify.com/) and you do..."
- `{{ | plus: Kelly }}`: "I don't know if you saw [JML's (Jean-Michel Lemieux) tweet](https://twitter.com/jmwind/status/1333834717704163330?lang=en) but JML is trying to do marketing and yeah 2021 we're gonna hire 2,021 new engineers, so yeah."
- `{{ Kelly | }}`: "The answer is, Yes."
- `{{ | plus: Kelly }}`: "The answer is yes. Final year student, look at the Shopify Intern Program, which should be on the careers page. You should be able to access that. You would be going through the Shopify Intern Program, if you want. Now winter it's closed, so you would be looking at for next fall. September is when it would start. You would going through interviews between now and april, something like that. Hope that's helpful."
- `{{ Kelly | }}`: "Cool."
- `{{ | plus: Kelly }}`: "Let's start building stuff. You did joined my collaborative session?!"
- `{{ Kelly | }}`: "I did. I am in there."
- `{{ | plus: Kelly }}`: "So let's open up the files. Of course I'm just teasing people that we're going to start building things, :laughing: :laughing:"
- `{{ Kelly | }}`: ":laughing: :laughing:"
- `{{ | plus: Kelly }}`: "One thing before we start building that I want to show. That I have installed on [Visual Studio Code (vscode)](https://code.visualstudio.com/) is this really cool new [vscode extension](https://marketplace.visualstudio.com/items?itemName=Shopify.theme-check-vscode) called `Theme-Check`. It's a [Shopify](https://www.shopify.com/) official vscode... Is this our first official vscode...?"
- `{{ Kelly | }}`: "I think so."
- `{{ | plus: Kelly }}`: "Do we have anything else? I think [CP (Charles-Philippe Clermont)](https://github.com/charlespwd) is the first to reach this ground for [Shopify](https://www.shopify.com/). Thank you [CP](https://simplified.dev/).
- `{{ Kelly | }}`: "Yeah, I do see somebody else using the name Shopify, but I do not believe that actually..."
- `{{ | plus: Kelly }}`: "Well this is a legitimate Shopify library. So this was thrown together by [Marc Cournoyer](https://twitter.com/macournoyer). He was hear in the stream earlier, don't know if he still here. However, this was a [Hack Days](https://www.shopify.com/partners/blog/18969895-why-hack-days-are-great-for-designers) product. I don't know if you remember I mentioned in December that we had [Hack Days](https://www.shopify.com/partners/blog/18969895-why-hack-days-are-great-for-designers) in December, which that's our internal hackathon where people stop what they're doing and work on any project that they really feel like working on and this is a Hack Days success story. There was a really good video that I wish could be made public. Hey!!! Marc is still here!!! I wish that Marc could share publicly. I don't know if you've seen [Powerthirst](https://www.youtube.com/watch?v=qRuNxHqwazs)... Let me seeif anyone in the audience has seen [Powerthirst](https://www.youtube.com/watch?v=qRuNxHqwazs). This is an old-school e-bomb's worlds viral video, like flash video. He did a great replication of it."
- `{{ Kelly | }}`: "I love that."
- `{{ | plus: Kelly }}`: " It had me in tears 😂... And now we're seeing it. It's its own [git](https://github.com/Shopify/theme-check), so let me pull... If you're interested in looking at the code or even contributing to it, it is open source. So, [Github `Theme-Check` Shopify](https://github.com/Shopify/theme-check). Let's see how the SEO is for this [repo](https://github.com/Shopify/theme-check). Look at that.."
- `{{ Kelly | }}`: "I did the same thing... [Github](https://github.com/Shopify/theme-check)"
- `{{ | plus: Kelly }}`: Read a comment, most likely from [Marc](https://twitter.com/macournoyer), saying "Lot's of yelling 🤣🤣"
- `{{ | plus: Kelly }}`: "So here's what the the vs code plugin is built on top of there is [another repo for the actual vscode plugin](https://github.com/Shopify/theme-check-vscode) but it's essentially wrapping what is the core linter that is here. So going through it's looking for syntax errors, json syntax errors, missing snippets and section templates, unused assigns..."
- `{{ Kelly | }}`: "uh, amazing"
- `{{ | plus: Kelly }}`: "from the javascript world that you're just used to having, now you can make sure you can clean up all those old dirtiest signs that you have laying around not getting used unused snippet templates it's going to tell you 'hey you got to snippet in here you don't even use it'..."
- `{{ Kelly | }}`: "'hey remember that app you uninstalled four years ago the theme code still exists."
- `{{ | plus: Kelly }}`: " it's still being loaded it's still here it's still slowing down your store'. Hashtag `#ghostapps`"
- `{{ Kelly | }}`: 🤣🤣
- `{{ | plus: Kelly }}`: "We're calling those ghost apps"
- `{{ Kelly | }}`: "They're ghost apps now. 🤣🤣"
- `{{ | plus: Kelly }}`: "They're ghost apps 🤣... Template lenght. I am wondering does this tell you if it's too long? I have to find out. Deprecated tags. That's really handy, for example the `snippets` have gone from the[ `{% include %}` you use to use to `{% include 'snippet-name' %}`](https://shopify.dev/docs/themes/liquid/reference/tags/deprecated-tags#include), via the `include` tag, and now it's the `render` tag, [`{% render 'snippet-name' %}`](https://shopify.dev/docs/themes/liquid/reference/tags/theme-tags#render).
- `{{ Kelly | }}`: "now, oh using theme check. Okay, I was going to say, because you can still use include, as it is still supported. So, all themes that are still using `{% include %}` are absolutely going to continue to work and function just fine. It will, however, yell at you if you try to use `{% render %}` and `{% include %}` in the same theme file."
- `{{ | plus: Kelly }}`: "Oh, really! When you upload?!"
- `{{ Kelly | }}`: "Yeah. It throws an error, at least it used too."
- `{{ | plus: Kelly }}`: "So, if I do `{% include 'test' %}` right there, now, when I tried tried this out it did have a slight delay. Little tiny little delay, it doesn't show instantly. There it is. There see, so now it says `{% include %}` is deprecated, convert it to `{% render %}`
- `{{ Kelly | }}`: "Nice!"
- `{{ | plus: Kelly }}`: "I love to see it how it's inline.
- `{{ Kelly | }}`:
- `{{ | plus: Kelly }}`:
- `{{ Kelly | }}`:
- `{{ | plus: Kelly }}`:
- `{{ Kelly | }}`:
- `{{ | plus: Kelly }}`:
- `{{ Kelly | }}`:
- `{{ | plus: Kelly }}`:
- `{{ Kelly | }}`:
- `{{ | plus: Kelly }}`:

<br>
### Legend

----

[Assets\img\t-kelly.jpg](https://twitter.com/kvlly)

- `{{ Kelly | }}` = [Kelly Vaughn](https://www.linkedin.com/in/kellyvaughn/)

[![4f9d4f51b887e1264249a8df7a595ba9.png](:/a0169c72c61a4ebcb0157841df70ba20)](https://twitter.com/thommaskelly)

- `{{ | plus: Kelly }}` = [Thomas Kelly](https://github.com/t-kelly)

----

### More Links

- Regex tutorial — A quick cheatsheet by examples: <https://medium.com/factory-mind/regex-tutorial-a-simple-cheatsheet-by-examples-649dc1c3f285>
- Regex cookbook — Top 10 Most wanted regex: <https://medium.com/factory-mind/regex-cookbook-most-wanted-regex-aa721558c3c1>
- Helium's Customer Fields App: <https://apps.shopify.com/customr?surface_detail=helium&surface_inter_position=1&surface_intra_position=5&surface_type=search>
- Shopify App CLI: <https://github.com/Shopify/shopify-app-cli>
- Youtube API: <https://developers.google.com/youtube/v3>
