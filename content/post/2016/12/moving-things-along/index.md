---
title: "Moving things along"
date: "2016-12-04"
categories: 
  - "reflection"
  - "web-dev"
tags: 
  - "css"
  - "design"
  - "html"
  - "javascript"
  - "label"
  - "navigation"
  - "portfolio"
  - "reflection"
---

This week's journal entry is short and sweet as I know what I need to do but I need to crack on and actually do it! My goal for this work-weekend is to try and get all of my [bits together in order to present a semblance of a whole](http://fionamacneill.co.uk/blog/2015/12/06/bits-pieces-put-together-to-present-a-semblance-of-a-whole/). Things that I have fixed/done this week...

1. **The irritating arrow scroll issue** when using keyboard keys to navigate the Flickity image carousel ([aria-labelled accessibility controls](https://www.w3.org/TR/wai-aria/states_and_properties#aria-label)). Solution: I created a new version of the flickity.js and found the section pertaining specifically to the accessibility controls (keycode == 39 and event.preventDefault<fn>Marcus gave me a hint for this one, but I needed to give the code a thorough mental and literal work through to ensure that I was putting it in the correct place.</fn>).
2. **Looked at the grid widths again**, I think that these are approaching completion. It will still be a big job to implement the grid on my new portfolio page.
3. **Started to sort out media queries**. Initially, I had thought that mobile first would be best, but considering the work domain of my primary user audience (nurses) it needs to operate optimally for desktop and be adjusted for mobile. My grid design will help to make this possible.
4. **Navigation** - I created a prototype version of the navigation. I am not particularly happy with it as it is reliant on browser respect of the z-index property in CSS. Firefox, Chrome and Internet Explorer 9 are respecting the layering, Safari is not. The navigation has been given a fixed position so that is floats down the page with the user. The navigation links take the user to different sections of the page<fn>sections are literally HTML 5 sections, this will require a bit of fix-up code for browsers that do not support that, e.g. [https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/Using\_HTML\_sections\_and\_outlines#Using\_HTML5\_elements\_in\_non-HTML5\_browsers](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/Using_HTML_sections_and_outlines#Using_HTML5_elements_in_non-HTML5_browsers)</fn>. I like the styling of [this navigation example on codepen](http://codepen.io/anon/pen/QGQPmX) and might see if I am do something more like this as my current navigation feels a bit retro (complete with a:active and a:hover).
5. **For the navigation transitions** I initially looked at whether I could reuse my work on the vanilla js smooth-scroll function. I did some reworking for the scrolling to work in the vertical, rather than horizontal but it proved unwieldy and did not work at all in Internet Explorer. After looking at a few options, almost all of them reliant on JQuery (as is the case with the navigation example above). I settled on [C. Ferdinandi's Smooth-Scroll script on github](https://github.com/cferdinandi/smooth-scroll) as it is based on vanilla.js and _span id_ which searches for a specified tag id. Something based on tag id as opposed to specified regions seems more durable as the regions will constantly change based on the responsive layout. I did encounter some issues with exactly where the _span id_ should be placed in relation to the sections. I'm sure that this is something that I can resolve by taking a closer look at the documentation.

### References

Adding z-index. (2015, September 3). Retrieved December 4, 2016, from [https://developer.mozilla.org/en-US/docs/Web/CSS/CSS\_Positioning/Understanding\_z\_index/Adding\_z-index](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Positioning/Understanding_z_index/Adding_z-index) The box model. (2016, October 10). Retrieved December 4, 2016, from [https://developer.mozilla.org/en-US/docs/Learn/CSS/Introduction\_to\_CSS/Box\_model](https://developer.mozilla.org/en-US/docs/Learn/CSS/Introduction_to_CSS/Box_model) Coyier, C. (2015, March 5). Creating responsive, touch-friendly carousels with Flickity. Retrieved December 4, 2016, from Article, [https://css-tricks.com/creating-responsive-touch-friendly-carousels-with-flickity/](https://css-tricks.com/creating-responsive-touch-friendly-carousels-with-flickity/) cferdinandi. (2016, September 23). Cferdinandi/smooth-scroll. Retrieved December 4, 2016, from [https://github.com/cferdinandi/smooth-scroll](https://github.com/cferdinandi/smooth-scroll) nav. (2015, October 27). Retrieved December 4, 2016, from [https://developer.mozilla.org/en-US/docs/Web/HTML/Element/nav](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/nav) Smooth anchor Scrolling. Retrieved December 4, 2016, from [http://codepen.io/anon/pen/QGQPmX](http://codepen.io/anon/pen/QGQPmX) w3.org. Accessible Rich Internet applications (WAI-ARIA) 1.0. Retrieved December 4, 2016, from [https://www.w3.org/TR/wai-aria/states\_and\_properties#aria-label](https://www.w3.org/TR/wai-aria/states_and_properties#aria-label) Yates, I. (2012, February 22). A simple, responsive, mobile First navigation. Retrieved December 4, 2016, from [https://webdesign.tutsplus.com/articles/a-simple-responsive-mobile-first-navigation--webdesign-6074](https://webdesign.tutsplus.com/articles/a-simple-responsive-mobile-first-navigation--webdesign-6074)
