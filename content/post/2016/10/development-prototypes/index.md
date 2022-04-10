---
title: "Development prototypes"
date: "2016-10-31"
categories: 
  - "journal-dev"
  - "reflection"
  - "web-dev"
tags: 
  - "accessibility"
  - "array"
  - "css"
  - "github"
  - "journal"
  - "plugins"
  - "reflection"
  - "themes"
  - "wordpress"
---

[A couple of posts back](https://fionamacneill.co.uk/post/2016/10/portfolio-site-concept-and-other-news/) I outlined some grand plans in terms of UX design documentation and artefacts that I am planning to put together. Don't worry I haven't forgotten about these things, but they are having to happen gradually alongside my formative code learning and experimentation, so they will be attached to future entries.

## Portfolio development

One thing I have learned from working in IT for 7+ years is that it is best not to say what you will build until you know what you can build. Sometimes this is knowing the right people who can build it for you, sometimes this is knowing the right tools to use in order to build. With this in-mind I decided to use a long weekend off work to create some coding prototypes to check if what I was envisioning in my mind is actually possible. This is completely opposite of what I would do with UX where I design the interface first without getting too attached to a specific technology. This is okay, but there is value in understanding what can be achieved, especially as I am doing it all myself!

### Prototype 1

My first prototype was a simple site based on the html5 <section> element[^1]. My thought was that in a later iteration it would resemble something like [the Akita site](http://www.akita.co.uk/computing-history/). Where container <div>s are added to the sections in order to align written and image-based content. I started by using header level ID tags as anchors for navigation through the content and then used the "tabindex" to determine navigation with the tab key. This prototype was fine, but I felt immediately frustrated by the jerkiness of the navigation; this would certainly take away from the experience of reading the content. 

<iframe src="https://www.youtube-nocookie.com/embed/8CQzRYzoM5s?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe>

### Prototype 2

I asked Marcus for some advice about how best to implement a script to support smooth navigation. I had already done quite a bit of Google searching for a solution to this, but everything that I found involved jQuery[^2]. There is nothing inherently wrong with jQuery, but I would prefer not to use any libraries for my site as it may impact loading time and time is crucial (as I said what I am creating is a _coffee break_ website). Also I want to make sure that the code as kept as clean as possible, so that I can see how it works in Internet Explorer 9. This is because unfortunately for me, the bulk of my end-users, use that web browser (an emoticon is unprofessional, but a frown-y face here would articulate my feelings). Marcus suggested that I include the search term "vanilla" and this did the trick. Helping me to find an excellent piece of script that I could adapt by P. Gryzybek ([see his blog post about it here](https://pawelgrzybek.com/page-scroll-in-vanilla-javascript/)) and [the codepen.io source](http://codepen.io/pawelgrzybek/pen/QEQoZL)). I have to admit that I did feel a bit guilty for adapting someone else's script, because I would like to have enough knowledge to create one from scratch on my own. However, at the moment my knowledge of the Javascript syntax is lacking a bit; essentially I know what I would like to do but I lack the right grammar to do it! So adapting other people's scripts, which I then cite in the comments is a good way to for me to learn. 

In prototype 2, shown below, buttons are used to trigger the smooth scrolling. The smooth scrolling function itself is based on moving between sections as parts of an array (Crockford, 2008, p.58). This is a clean way of doing it as there is a clear chronology and index in the array and the scrolling movement reflects that. However, the array also meant that I needed to rethink my structure and consider naming properties carefully. For example, in the original script the parts of the array were called "sections" I knew immediately that I had to change that as I planned to use HTML5 sections, so having "sections" in the javascript would become confusing for anyone who needed to review my code later on. Therefore I changed that aspect to be "parts" in the .js file. 

I decided to introduce a new series of buttons with the purpose of moving from section to section of the site. These "Next" buttons use the same javascript "scrollIt" function but are independent from the section navigation buttons that float at the top-left, this will allow me to style them separately in the CSS later on. The arrays were both useful and frustrating as there are 12 "Next" buttons, whereas there are 13 sections (0-12) in the sections/parts array. This means that the "Next" buttons need to be staggered, so the "Next" button indexed at "0" points to "1", and "1" points to "2" and so on and so forth. This is a downside of reusing the ScrollIt function's array but better than adding another layer of script to run through. 

The other thing that I spent way too much time on is trying to add keyboard-based navigation to prototype 2. I tried a few approaches including a [_Switch_](https://developer.mozilla.org/en-US/docs/switch_command_JavaScript) (this was most effective) picking up the values of the up (=38) and down (=40) keyCode values. I also tried to construct _if _and _[do...while](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/do...while)_ statements in javascript. However, try as I might I could not get the repeated use of the down key to keep going down the list, I could only get it going down to the second position and then it got stuck. I will need to seek advice on this and come back to it. 

<iframe src="https://www.youtube-nocookie.com/embed/fRcH_KIdhmE?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe>

Having said all this, I am pretty happy with prototype 2 as a starting point and I feel that it can provide the structure needed for the next steps. So NOW I am ready to do more on wireframing and possibly physical prototyping. As a start for the creation of these prototypes I used the [HTML5 Boilerplate](https://html5boilerplate.com/) that is available on GitHub. It seemed like a good way of familiarising myself with all the parts that would be needed for a fully fledged HTML5 application. There are many template parts that I will likely discard, but it was certainly helpful to start this way and it provided a logical filing structure. My new GitHub repository specifically for [the portfolio project can be found here](https://github.com/FionaMacNeill/portfolioproj). I also added a Normalize.css file based on [this template from GitHub](https://necolas.github.io/normalize.css/5.0.0/normalize.css). Based on Marcus's session this week, it is a good idea to include a normalize.css file as it standardises the browsers' built-in interpretation of styles.

## Journal developments

I asked Marcus for some advice on the background colour changing widget (aka stylesheet switcher) and he felt that loading images for the colour-change buttons added to the processing load. I tried a few things in the MAMP version of this journal on my development computer, including changing the images to 1 pixel and then also trying to create _buttons_ that could just be a colour and not a jpeg or png image file. None of these things worked well and I came to the conclusion that as I am working with a plugin and some of these tweaks broke the plugin, I just need to handle the plugin's limitations. As I don't have enough time to build my own plugin, I decided to made the images small and simple at 20px x 20px and then altered the stylesheet to make the layout more uniform so that they fit into the sidebar widget better and are shown in a row at most browser window sizes (the widget disappears at phone screen size, this is intentional in the Twentysixteen parent theme, to avoid clutter). In addition, I added a piece of loading script at the top of each colour-option CSS file as I need each one to load the child theme's CSS, so that I don't need to make changes to all of the CSS files, only the main child theme version. I mapped the stylesheet switcher plugin's php to look in the "css" folder, but I also found that the main child style.css file needed to live in the root folder in order to operate properly (thank you Google Chrome console for highlighting this issue!). A further development for the stylesheet switcher will be to look at the default hyperlink colours in relation to each background. This includes their active, inactive and visited states as the contrast in relation to the background colour needs to be readable for each colour. 

### Additional considerations:

- Do I want to provide a choice of fonts and if so, would I provide that function via a different plugin?
- I should look at installing the [accessibility plugin](https://en-gb.wordpress.org/plugins/wp-accessibility/) and investigating the best settings.

## Development log

It struck me that I am adding a lot of short notes and written updates to GitHub. I felt like it would be good to maintain a digest of these changes and thoughts in this journal, alongside my longer form writing. Therefore I did a bit of searching and found [information about the atom feeds for "commit" changes](http://stackoverflow.com/questions/7353538/setting-up-an-github-commit-rss-feed])). In order to display this feed, I needed an aggregator. I selected the [CyberSyn plugin](https://wordpress.org/plugins/cybersyn/) as it has been updated recently and offers excellent functionality. However, as the GitHub commit posts are a bit code-like and lacking correct grammar, I don't want them on the front page of this journal but [in their own category](http://fionamacneill.co.uk/blog/category/dev-log/). So I set the CyberSyn plugin to set all feed posts as a new "development log" category and used the [Ultimate Category Excluder plugin](https://wordpress.org/plugins/ultimate-category-excluder/) to omit that category from the front page posts feed. I'm pretty happy with that!

## References

Crockford, D. (2008)._JavaScript: The good parts._ Sebastopol, CA, USA: O'Reilly Media. Lawson, B., & Sharp, R. (2012). _Introducing HTML 5 second edition._ Berkley, CA, USA: New Riders.

[^1]: Learned about this from pp. 18-19 and p.54 of the Introducing HTML 5 book (Lawson & Sharp, 2012).

[^2]: [For example this post on StackOverflow](http://stackoverflow.com/questions/6677035/jquery-scroll-to-element/6677069#6677069)
