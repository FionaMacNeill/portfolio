---
title: "Theme testing"
date: "2016-10-13"
categories: 
  - "journal-dev"
  - "reflection"
tags: 
  - "accessibility"
  - "css"
  - "github"
  - "javascript"
  - "plugins"
  - "theme"
---

This journal entry continues on from the section, "[First thoughts related to this journal site](https://fionamacneill.co.uk/post/2016/10/hello-world-the-epitome-of-the-inaugural-blog-post/)" in my first post. In that section I outlined plans to test a number of WordPress themes that had been tagged with accessibility. This led me down a fascinating path of learning with one wrong turn along the way.

### The testing process

In my last post I outlined a number of themes that looked like possible candidates, including the following:

1. [afterlight (Automattic, 2015)](https://wordpress.org/themes/afterlight/)
2. [chuchadon (Keijonen, 2016a)](https://wordpress.org/themes/search/chuchadon/)
3. [e-nigma (Lüken, 2015)](https://wordpress.org/themes/e-nigma-2015/)
4. [kuorinka (Keijonen, 2016b)](https://wordpress.org/themes/kuorinka/)
5. [twentyfifteen (WordPress.org, 2016a)](https://wordpress.org/themes/twentyfifteen/) (WordPress core theme)
6. [twentysixteen (WordPress.org, 2016b)](https://wordpress.org/themes/twentysixteen/) (WordPress core theme)

As part of the testing plan I used a several tools, listed at the bottom of this post, to analyse the best themes. Please note, that some themes did not reach the full testing phase due to issues that I would term as _deal breakers_; the issues identified were troublesome enough where it was not worth continuing with those themes. I also entered into this testing process with an intention to attain a WCAG 2.0 Level AA (W3C, 2016a) accessibility rating for my journal site. This is largely because accessibility is a budding specialism of mine and I wanted an excuse to delve around in the innards of the newest WordPress themes!

#### Testing results and observations

1. [afterlight](https://wordpress.org/themes/afterlight/) I decided not to install this theme. Although 'afterlight' had the accessibility tag, I found on inspection of its specifications that it is based on having a background image throughout each area of its architecture (landing page, pages, posts - all had to have a single background image). Upon previewing this with my content, using the WordPress theme preview tool, I found that this negatively impacted readability. As the purpose of this blog is to engage in reflection, it seems important not to distract from that at the design level.

2. [chuchadon](https://wordpress.org/themes/search/chuchadon/) This theme has (or rather had) a lot of potential and is coded according to best practice (e.g. accessibility tagging) outlined in the WordPress Accessibility Handbook (WordPress.org, 2014).
   
    I realised later on looking at in-code documentation that this theme is based on a starter theme, Underscores (or “\_s”). A bare bones CSS starter theme (Underscores, 2016).
   
    Unfortunately after venturing as far as creating a child theme, I found issues in the some of the front-page template functionality. I also discovered that the links through to the theme documentation were broken and as a result I decided cease using the theme.

3. [e-nigma](https://wordpress.org/themes/e-nigma-2015/) I do like the clean lines and simplicity of enigma, even in light of the negative points outlined in the slideshow below, it is certainly a worthy candidate. However, the dependence on the burger-style menu (the three lines) although often essential on mobile versions of a site, is less effective when viewed in a conventional web browser. I decided to seek out a theme that offered more versatility for delivery of the navigation menu/s.

4. [kuorinka](https://wordpress.org/themes/kuorinka/) Initially I really liked the simplicity of this theme design and it is very responsive, however in terms of accessibility it has some problems. Namely, it does not support reader view in Firefox 49 or Safari 10 and also was not good in terms of respecting the heading levels for the screen reader. I did not complete the other tests as these two issues were deal breakers.

5. [twentyfifteen](https://wordpress.org/themes/twentyfifteen/)
   
    The ultimate in clean and simple. Although as a seasoned WordPress user the annual core template always _looks_ like the annual core template, even with customisation. Twentyfifteen is quite book-like in its bi-fold layout and this doesn't strike the desired tone. As I tend to be quite verbose in my writing, I think that a theme with better except support is better. Having said that, the core templates can provide excellent bases for creation of child themes.

6. [twentysixteen](https://wordpress.org/themes/twentysixteen/) A fresh approach to a traditional blog layout with some very nice built-in features. Highlights include the support of the _read more_ tag for determining the length of post/entry excerpts shown on the front page. I also like the presentation of the author avatar, together with post tags on the left-hand side of each post. This theme has good customisation options and good widget support (the tools that you can place in the aside-style columns in the layout). A solid theme, not the most riveting to look at, but it ticks all of my accessibility boxes!
   
   ##### The final two contenders
   
    I ran an IDI web accessibility check and used Firefox accessibility checker plugin (SEE [tools section](http://fionamacneill.co.uk/blog/2016/10/13/theme-testing/#tools) for links) to enable keyboard control on the two top candidates: twentysixteen and chuchadon. Twentysixteen had two flagged elements when I looked at the posts page specifically - one was that h1 header element was nested, so the order of headers was not ideal. Also there was a missing label element in the search field. These would both be very easy fixes.
   
    Chuchadon had the same flag on the header nesting for a posts page, so it is likely that this is an issue that would be picked up for a number of WordPress based blog template. To test this theory I tested my own blog, which is based on the Edublogs implementation of WordPress. Interestingly this was not an issue on my blog (e.g. post: [MacNeill, 2016](http://fionamacneill.co.uk/blog/2016/06/14/trust-in-iot-app-interfaces-redux/)) or another Edublog that I tried. I took a look at the .entry-title tag in the edublog and it was at h2 level rather than h1. This struck me as an issue with both these themes. So I created a child theme of Chuchadon to try out a tweak on line 353 of the CSS stylesheet. The tweak worked perfectly, but alas this was also when I realised that there were some other things that didn't work for me in chuchadon (front-page configuration and the documentation links).
   
   ##### The final verdict
   
    I have selected twentysixteen as my theme and have created a child theme to allow more space for customisation. \[caption id="attachment\_324" align="alignnone" width="840"\][![Screenshot of the Twenty Sixteen theme](images/twentysixteen_img-1024x768.png)](http://fionamacneill.co.uk/blog/2016/10/13/theme-testing/twentysixteen_img/) Image source: WordPress.org, [https://wordpress.org/themes/twentysixteen/](https://wordpress.org/themes/twentysixteen/)  
    (Worpress.org, 2016b)\[/caption\] **Just to clarify...** You may be asking, what is all this talk of child themes. Well in essence a child theme is augmented version of it's original parent. Essentially a child theme allows you to commit edits to the visual presentation as well as the functions of a WordPress site without editing the original theme's code. This is a smart tactic for customising a theme, particularly the core annual themes, as because WordPress as a CMS has frequent updates, any accompanying parent theme updates can be safely run without affecting the code in the child theme too much. The use of a child theme will also allow me to replace the parts of the CSS and theme functions that were identified in the IDI accessibility report.

##### Techie stuff

The server was down this weekend so I used this as an excuse to implement some technical tools which will help further down the line. First of all as I mentioned in my last entry I installed MAMP on my development computer. MAMP, stands for Macintosh, Apache, MySQL, PHP ("MAMP", 2016) and allows to setup a local copy of WordPress on your computer. I find having access to a local installation to be helpful for two reasons:

- I can work on my child theme tweaks without having access to the server and test them out in a controlled environment.
- I can test out themes and plugins without muddying my installation. Sometimes everything about a plugin can look good and then you install it and there are things are about it that don't work or the coding isn't up to scratch. So again it is good to have a test environment for that.

I also setup a github repository for version control; to track my changes to the theme files. This is the first time that I have setup my own repository, so it was definitely a learning curve for me. However, I think that knowing how to do this will be essential for my forthcoming work on my web portfolio project. Here is my repository for this site: [https://github.com/FionaMacNeill/learningjournal](https://github.com/FionaMacNeill/learningjournal) - it seemed like the ideal opportunity to practice using a version control tool. It has been really useful thus far! **Thinking long and hard about plugin installation is a good idea...** I was right to spend time deliberating about the types of plugin to install. The problem with plugins is that you often have to spend time tweaking them for every update and every theme. My carefully considered decision to install the footnotes plugin has already had to result in CSS tweaks<fn>Why not use a footnote to explain what I did! I changed .footnote\_plugin\_text to change the width of the area where the footnotes are shown and the font size. I also had to make the table border elements transparent in the .footnote\_plugin\_link, .footnote\_plugin\_index. Finally I needed to manually change the position of the superscript figures as I wasn't happy with the distance of the figure numbers from the text characters, for this I changed the .footnote\_plugin\_tooltip\_text class</fn> due to how the footnotes were shown in the twentysixteen theme.

* * *

##### **Analysis tools used:**

- IDI Web Accessibility checker (AChecker, 2011).
- Snook colour contrast checker (Snook, 2015).
- Sim Daltonism colour blindness simulator (Wickline, 2000).
- Accessibility evaluation toolbar by John Gunderson (Gunderson, 2011).
- Apple and Firefox text-to-speech tools.
- Keyboard-only navigation of site.

##### **Guidelines used and referred to:**

- Web Content Accessibility Guidelines (WCAG) (W3C, 2016a).

- Techniques for WCAG 2.0 (W3C, 2016b).

- BBC Future Media Standards and Guidelines (BBC, 2008).

- Mozilla Developer Network documentation (Mozilla, 2016).

- WordPress Accessibility Handbook (WordPress.org, 2014):
  
  - Specifically I found this page very helpful - Questions to ask - [https://make.wordpress.org/accessibility/handbook/accessibility-overview/which-questions-should-you-ask/](https://make.wordpress.org/accessibility/handbook/accessibility-overview/which-questions-should-you-ask/) The 'questions' are derived from the four principles of WCAG and they are immensely helpful.

##### **Software and developer tools used****:**

- MAMP (appsolute GmbH, 2016).
- Github - version control and code repository (GitHub, 2016).
- WebStorm - editor: (JetBrains, 2016).
- Textwrangler (Bare Bones Software, 2016).
- Chrome developer tools (Google, 2016).

 

#### References

AChecker. (2011). IDI web accessibility checker: Web accessibility checker. Retrieved October 7, 2016, from AChecker website, [http://achecker.ca/checker/index.php](http://achecker.ca/checker/index.php)

appsolute GmbH. (2016). MAMP & MAMP PRO. Retrieved October 7, 2016, from MAMP website, [https://www.mamp.info/en/](https://www.mamp.info/en/)

Automattic. (2015, October 7). Afterlight. Retrieved October 7, 2016, from Wordpress.org website, [https://wordpress.org/themes/afterlight/](https://wordpress.org/themes/afterlight/)

Bare Bones Software. (2016). Bare bones software. Retrieved October 13, 2016, from [http://www.barebones.com/products/TextWrangler/](http://www.barebones.com/products/TextWrangler/)

BBC. (2008, June 24). Future media standards & guidelines - accessibility guidelines v2.0. Retrieved October 7, 2016, from BBC website, [http://www.bbc.co.uk/guidelines/futuremedia/accessibility/](http://www.bbc.co.uk/guidelines/futuremedia/accessibility/)

GitHub. (2016). Build software better, together. Retrieved October 13, 2016, from [https://github.com/](https://github.com/)

Google. (2016). Chrome DevTools overview - Google chrome. Retrieved October 13, 2016, from [https://developer.chrome.com/devtools](https://developer.chrome.com/devtools)

Gunderson, J. (2011, August 19). Accessibility evaluation Toolbar. Retrieved October 13, 2016, from [https://addons.mozilla.org/en-US/firefox/addon/accessibility-evaluation-toolb/](https://addons.mozilla.org/en-US/firefox/addon/accessibility-evaluation-toolb/)

Herbert, C. (2016, October 8). Where does “hello world” come from? \[Online forum comment\]. Retrieved from StackOverflow website: [http://stackoverflow.com/questions/602237/where-does-hello-world-come-from](http://stackoverflow.com/questions/602237/where-does-hello-world-come-from)

JetBrains. (2016). WebStorm: The smartest JavaScript IDE. Retrieved October 13, 2016, from [https://www.jetbrains.com/webstorm/](https://www.jetbrains.com/webstorm/)

Keijonen, S. (2016a, September 16). Chuchadon. Retrieved October 7, 2016, from WordPress.org website, [https://wordpress.org/themes/chuchadon/](https://wordpress.org/themes/chuchadon/)

Keijonen, S. (2016b, December 29). Kuorinka. Retrieved October 7, 2016, from WordPress.org website, [https://wordpress.org/themes/kuorinka/](https://wordpress.org/themes/kuorinka/)

Lüken, A. (2015, October 31). E.Nigma 2015. Retrieved October 7, 2016, from WordPress.org website, [https://wordpress.org/themes/e-nigma-2015/](https://wordpress.org/themes/e-nigma-2015/)

MacNeill, F. (2016, June 14). \[Talk\] factors of trust in IoT App interfaces Redux \[Blog post\]. Retrieved from [http://fionamacneill.co.uk/blog/2016/06/14/trust-in-iot-app-interfaces-redux/](http://fionamacneill.co.uk/blog/2016/06/14/trust-in-iot-app-interfaces-redux/)

Mozilla. (2016). Mozilla developer network. Retrieved October 13, 2016, from [https://developer.mozilla.org/en-US/](https://developer.mozilla.org/en-US/)

MAMP. (2016, September 29). In _Wikipedia._ Retrieved October 16, 2016 from [https://en.wikipedia.org/wiki/MAMP](https://en.wikipedia.org/wiki/MAMP)

Rietveld, R. (2016, March 21). WordPress goes WCAG \[Blog post\]. Retrieved from [https://make.wordpress.org/accessibility/2016/03/21/wordpress-goes-wcag/](https://make.wordpress.org/accessibility/2016/03/21/wordpress-goes-wcag/)

Snook. (2015, January 11). Snook colour contrast checker. Retrieved October 13, 2016, from Snook.ca website, [https://snook.ca/technical/colour\_contrast/colour.html#fg=33FF33,bg=333333](https://snook.ca/technical/colour_contrast/colour.html#fg=33FF33,bg=333333)

Underscores. (2016). Retrieved October 7, 2016, from Underscores website, [http://underscores.me/](http://underscores.me/)

W3C. (2016a). How to Meet WCAG 2.0. Retrieved October 13, 2016, from W3C Web Accessibility Initiative website, [https://www.w3.org/WAI/WCAG20/quickref/](https://www.w3.org/WAI/WCAG20/quickref/)

W3C. (2016b). Techniques for WCAG 2.0. Retrieved October 13, 2016, from W3C Working Group website, [https://www.w3.org/TR/WCAG20-TECHS/](https://www.w3.org/TR/WCAG20-TECHS/)

Wickline, M. (2000). Sim Daltonism for Mac. Retrieved October 13, 2016, from [https://michelf.ca/projects/mac/sim-daltonism/](https://michelf.ca/projects/mac/sim-daltonism/)

WordPress.org. (2014, October 11). Accessibility handbook. Retrieved October 7, 2016, from WordPress.org website, [https://make.wordpress.org/accessibility/handbook/](https://make.wordpress.org/accessibility/handbook/)

WordPress.org. (2016a, December 6). Twenty Fifteen. Retrieved October 7, 2016, from WordPress.org website, [https://wordpress.org/themes/twentyfifteen/](https://wordpress.org/themes/twentyfifteen/)

WordPress.org. (2016b, December 6). Twenty Sixteen. Retrieved October 7, 2016, from Wordpress.org website, [https://wordpress.org/themes/twentysixteen/](https://wordpress.org/themes/twentysixteen/)
