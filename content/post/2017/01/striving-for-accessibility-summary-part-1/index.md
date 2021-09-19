---
title: "Striving for accessibility - Eval pt 1"
date: "2017-01-19"
categories: 
  - "reflection"
  - "web-dev"
tags: 
  - "accessibility"
  - "compliance"
  - "css"
  - "interactive"
  - "reflection"
  - "research"
  - "responsive"
  - "screenreader"
---

Part 1 of my final evaluation. This entry outlines key decisions that I made regarding accessibility towards the end of the development period. I am writing and publishing it retroactively as it as represents a very large amount of thinking and work, which I kept notes about as I went along.

### Based on observation

Based on looking at a large number of NHS and governmental sites, referenced in former posts I realise that accessibility is crucial, perhaps even more than your average portfolio site. For example, looking at NHS England (2017) site I see that they offer a text-to-speech service. Based on experience in my day-job working with software vendors, some of these solutions can be quite expensive. It was however important to me to make the site as accessible as possible and that has meant some sacrifices along the way.

### Keystone texts

While engaging in this in-depth investigation into the accessibility, I found myself referring to the following keystone texts.

- [Accessible Rich Internet Applications (WAI-ARIA) Roles Model (n.d.)](https://www.w3.org/TR/wai-aria/roles)
- [The Paciello group's blog](https://www.paciellogroup.com/blog/) - UX accessibility specialists an amazing resource
- [Mozilla Developer Network Accessibility Guides](https://developer.mozilla.org/en-US/docs/Learn/Accessibility)
- [The Nielsen Norman Group blog](https://www.nngroup.com/articles/) - a frequent go-to of mine

I feel like I have only scratched the surface with the WAI-ARIA roles, but based on testing I feel that the site is accessible as I could get it within the allotted time. In the end I found a blog post on the subject by a rather brilliant developer, Aaron Krauss (2016) who did a great job of how to practically use certain ARIA labels and roles. What I did find is that there is quite a lot of redundancy in the code, but you need to have it there as the screenreader doesn't necessarily pick up the semantics in the page construction as you might intend. Here is a video of my screenreader testing in action with tab key only - tabindex (Mozilla Developer Network, 2017)

<iframe style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;" src="https://mediastream.brighton.ac.uk/player?autostart=n&amp;fullscreen=y&amp;width=0&amp;height=0&amp;videoId=6936&amp;quality=hd&amp;captions=n&amp;chapterId=0" width="300" height="150" frameborder="0" scrolling="no"></iframe>

### What the font?

I conducted some reading (Nielsen, 2002; Martin, 2009; Franz, 2014; ) around legible fonts and font sizes and optimal line height. I have tried my best to work with the best practices, although that does get tricky with the mobile screen size. However, the attention that I have paid to optimising the CSS stylesheet for plain readers should help those who use accessibility features on mobile devices. **Added a fix to the superscript** I found a very helpful snippet for fixing line height for superscript (used for references) and subscript. Thank you to the -ever helpful- CSS Tricks site (Coyier, 2009a). **Contrast** As much as I loved the white headers along the timeline the contrast was not sufficient. The colour scheme is themed around blues and purples and unfortunately white on blue doesn't comply with WCAG 2.0 unless the blue shade is very dark or the white font is very large (Snook, 2015; WAVE, n.d.).

### The accordion had to go

Upon testing the tab-key only navigation I realised that there was no accessible way (that I could muster anyway) to navigate the accordion (Mary Lou, 2012) and for that reason it had to go. I added two simple tables, which I was trying to avoid, but as they area features comparisons this use us permissible. I was not using the tables for layout, but for the display of information in a standardised way. After the fact I found this accordion example at codepen.io which might have been better, but not without a lot of work: [https://codepen.io/stowball/pen/eZKwRv](https://codepen.io/stowball/pen/eZKwRv)

### Sprite fun

I got my sprite on and added sprites for the device images. The device images were drawings that I created in Adobe Illustrator based on photographs. All the photos were [CC0 - public domain](https://creativecommons.org/publicdomain/zero/1.0/deed.en) apart from the image of jeans, which I have listed below. This was added as an image through the CSS and aria-labelled for descriptive purposes. \[caption id="attachment\_393" align="alignnone" width="300"\][![Image of sprite file showing the wearable devices](images/devicediagrams-300x122.png)](http://fionamacneill.co.uk/blog/2017/01/19/striving-for-accessibility-summary-part-1/devicediagrams/) The complete sprite for the devices in all of its glory\[/caption\] Photograph used as the basis for illustration of fasten/clip wearable - ["My fave jeans copied"](https://flic.kr/p/5Rtzsu "Link to image at Flickr.com") by [ inger maaike](https://www.flickr.com/photos/ingermaaike2/ "Link to photographer page at Flickr.com") is licensed under [CC BY 2.0](https://creativecommons.org/licenses/by/2.0/ "Link to CC license") CC0 images sources from Pixabay: [https://pixabay.com/en/fingers-hand-pebbles-ring-1842661/](https://pixabay.com/en/fingers-hand-pebbles-ring-1842661/) [https://pixabay.com/en/apple-watch-smartwatch-watch-828827/](https://pixabay.com/en/apple-watch-smartwatch-watch-828827/) [https://pixabay.com/en/gold-neck-necklaces-style-792002/](https://pixabay.com/en/gold-neck-necklaces-style-792002/)

### Fixing the tab svg

I replaced the svg tab to be a proper thing rather than the Frankenstein's monster-like CSS creation [I outlined in an earlier journal entry](http://fionamacneill.co.uk/blog/2017/01/07/charty-mccharterson/). Once again I referred to the excellent CSS-Tricks (Coyier, 2013) and Mozilla Developer Network resources (2016c), as well as the Implementing Responsive Design book from the reading list (Kadlec, 2012).

### Asking myself questions

I tried my best to standardise all the units in the CSS although if I were to do it all again with hindsight I think that I might design my grid to work with ems or rems (once they are widely compatible or older browsers fall out of use). I'm sure that I have missed things in spite of several thorough read-throughs. It all validated okay. **CSS code block structure:** e.g. div class or id - this resembles the layout of a div .div { display: block; position: relative; width: 90% height: 60% color: #000; margin: 2% auto 2% auto padding: 2% 4%; (shortenings used where possible) } e.g. typography class or id - this resembles the layout h2 { font-family: "Helvetica Neue", Helvetica, Arial, sans-serif; text-align: center; font-size: 1.5em; line-height: 1.25; font-weight: 300; } In the HTML where white-space pre-line formatting was needed for the Goals and the references sections, I included comments to help indicate why the formatting was different in the markup. Also regarding the CSS as I was going through it, to weed it a bit, I asked myself a series of questions to help determine which units to use and such. I have included these below.

1. Is it text? = ems
2. If it moves it is em or %. If it doesn't or cannot move it is pixels
3. Is it in a column in the grid - then margins and padding are percentages (unless there is a very good reason for them not to be)
4. Is it in the grid - then margins and padding are percentages
5. Is it used in the html? No, then get rid of it Could it be consolidated in any way? Does it share the same values as another class and/or id?<fn>I would have liked to do more on this, but I ran out of time. Did my best to do it as I went along.</fn>
6. Does it need to be a negative value (particularly in the media queries)? Then it is in ems.

**Rationale:**

- When it is something that needs to have set dimensions such as a button, I am using pixels.
- For text I am using ems to ensure compatibility with older browsers
- For table related items and blocks which reside in divs I have used percentages.
- Used hexadecimal shortenings when it made sense to do so and it did not change the hue of the colour (three digits rather than the standard 6). I prefer digits rather than word descriptions, due to colour precision.

### Media queries

Did a lot of work on these, again I found the Implementing Responsive Design (Kadlec, 2012) and the Introducing HTML 5 (Lawson & Sharp, 2011) books particularly helpful. I also added a arrow keys image and tooltip to help explain the navigation of the timeline. You will notice for the tabbed navigation of the site in the screen reader demo that the timeline is skipped over initially and I added to the JavaScript in order to allow the tab key for navigation in addition to the arrow keys. The arrow keys allow for greater freedom though, as once you have started tabbing through the carousel/timeline, you cannot get out of it with another tab press. Thus leaving it to the end and this is something for me to raise with the original developers to see if they can address that in future versions of the widget.

#### References

 

Coyier, C. (2009a, August 10). Prevent Superscripts and subscripts from affecting line-height \[Blog post\]. Retrieved from [https://css-tricks.com/snippets/css/prevent-superscripts-and-subscripts-from-affecting-line-height/](https://css-tricks.com/snippets/css/prevent-superscripts-and-subscripts-from-affecting-line-height/)

Coyier, C. (2009b, October 24). CSS Sprites: What they are, why they’re cool, and how to use them \[Blog post\]. Retrieved from [https://css-tricks.com/css-sprites/](https://css-tricks.com/css-sprites/)

Coyier, C. (2013, December 4). SVG tabs (using an SVG shape as template) \[Blog post\]. Retrieved from [https://css-tricks.com/svg-tabs-using-svg-shape-template/](https://css-tricks.com/svg-tabs-using-svg-shape-template/)

Donut. (2011). Re: What are the most common font-sizes for H1-H6 tags. StackOverflow website. Retrieved 19 January 2017, from [http://stackoverflow.com/questions/6140430/what-are-the-most-common-font-sizes-for-h1-h6-tags#6140504](http://stackoverflow.com/questions/6140430/what-are-the-most-common-font-sizes-for-h1-h6-tags#6140504)

Franz, L. (2014, September 29). Size matters: Balancing line length and font size in responsive web design – smashing magazine \[Blog post\]. Retrieved from [https://www.smashingmagazine.com/2014/09/balancing-line-length-font-size-responsive-web-design/](https://www.smashingmagazine.com/2014/09/balancing-line-length-font-size-responsive-web-design/)

Kadlec, T. (2012). Responsive Media. In Implementing responsive design: Building sites for an anywhere, everywhere web (pp. 95–127). Berkeley, CA: New Riders Publishing.

Krauss, A. (2016, September 8). ARIA roles and attributes: How to actually use them | Aaron Krauss Retrieved from [https://thesocietea.org/2016/09/aria-roles-and-attributes-how-to-actually-use-them/](https://thesocietea.org/2016/09/aria-roles-and-attributes-how-to-actually-use-them/)

Lawson, B. D., & Sharp, R. (2011). Introducing HTML5 (2nd edition) (2nd ed.). Berkeley, CA: New Riders Publishing.

Martin, M. (2009, August 20). Typographic design patterns and best practices – smashing magazine \[Blog post\]. Retrieved from [https://www.smashingmagazine.com/2009/08/typographic-design-survey-best-practices-from-the-best-blogs/](https://www.smashingmagazine.com/2009/08/typographic-design-survey-best-practices-from-the-best-blogs/)

Mary Lou. (2012, February 21). Accordion with CSS3 \[Blog post\]. Retrieved from [https://tympanus.net/codrops/2012/02/21/accordion-with-css3/](https://tympanus.net/codrops/2012/02/21/accordion-with-css3/)

Mozilla Developer Network. (2015, July 23). Using the aria-describedby attribute. Retrieved January 19, 2017, from Mozilla Developer Network website: [https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/ARIA\_Techniques/Using\_the\_aria-describedby\_attribute](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/ARIA_Techniques/Using_the_aria-describedby_attribute)

Mozilla Developer Network. (2016a, December 15). WAI-ARIA basics. Retrieved January 19, 2017, from Mozilla Developer Network website: [https://developer.mozilla.org/en-US/docs/Learn/Accessibility/WAI-ARIA\_basics](https://developer.mozilla.org/en-US/docs/Learn/Accessibility/WAI-ARIA_basics)

Mozilla Developer Network. (2016b, November 17). CSS values and units. Retrieved January 19, 2017, from Mozilla Developer Network website: [https://developer.mozilla.org/en-US/docs/Learn/CSS/Introduction\_to\_CSS/Values\_and\_units](https://developer.mozilla.org/en-US/docs/Learn/CSS/Introduction_to_CSS/Values_and_units)

Mozilla Developer Network. (2016c, December 3). Background-position. Retrieved January 19, 2017, from Mozilla Developer Network website: [https://developer.mozilla.org/en-US/docs/Web/CSS/background-position](https://developer.mozilla.org/en-US/docs/Web/CSS/background-position)

Mozilla Developer Network. (2017, January 16). Tabindex. Retrieved January 19, 2017, from Mozilla Developer Network website: [https://developer.mozilla.org/en-US/docs/Web/HTML/Global\_attributes/tabindex](https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes/tabindex)

NHS England. (2017). About NHS England. Retrieved January 23, 2017, from NHS England website: [https://www.england.nhs.uk/about/](https://www.england.nhs.uk/about/)

Nielsen, J. (1996, October 1). Accessible design for users with disabilities \[Blog post\]. Retrieved from [https://www.nngroup.com/articles/accessible-design-for-users-with-disabilities/](https://www.nngroup.com/articles/accessible-design-for-users-with-disabilities/)

Nielsen, J. (2002). Let users control font size \[Blog post\]. Retrieved from [https://www.nngroup.com/articles/let-users-control-font-size/](https://www.nngroup.com/articles/let-users-control-font-size/)

Snook. (2015). Colour Contrast Check \[Computer software\]. Retrieved 19 January 2017, from [https://snook.ca/technical/colour\_contrast/colour.html#fg=33FF33,bg=333333](https://snook.ca/technical/colour_contrast/colour.html#fg=33FF33,bg=333333)

Stanford University Online Accessibility Program. (2016, August 1). Screen reader testing. Retrieved January 19, 2017, from Stanford University website: [https://soap.stanford.edu/tips-and-tools/screen-reader-testing](https://soap.stanford.edu/tips-and-tools/screen-reader-testing)

W3C. (2016, October 27). Accessible Rich Internet Applications (WAI-ARIA) 1.1 W3C Candidate Recommendation 27 October 2016. Retrieved January 23, 2017, from W3C website, [https://www.w3.org/TR/wai-aria-1.1/](https://www.w3.org/TR/wai-aria-1.1/)

W3C. The Roles Model. Retrieved January 19, 2017a, from WAI-ARIA website: [https://www.w3.org/TR/wai-aria/roles](https://www.w3.org/TR/wai-aria/roles)

W3C. WAI-ARIA role definition model - image. Retrieved January 19, 2017b, from WAI-ARIA website: [https://www.w3.org/TR/wai-aria/rdf\_model.png](https://www.w3.org/TR/wai-aria/rdf_model.png)

W3Schools. CSS Tooltip. Retrieved January 19, 2017, from w3schools.com website: [http://www.w3schools.com/css/css\_tooltip.asp](http://www.w3schools.com/css/css_tooltip.asp)

Watson, L. (2014, August 4). Using the tabindex attribute \[Blog post\]. Retrieved from [https://www.paciellogroup.com/blog/2014/08/using-the-tabindex-attribute/](https://www.paciellogroup.com/blog/2014/08/using-the-tabindex-attribute/)

WAVE web accessibility tool. \[Computer software\]. Retrieved January 19, 2017, from [http://wave.webaim.org/](http://wave.webaim.org/)
