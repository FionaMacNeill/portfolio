---
title: "Navigation"
date: "2016-12-26"
categories: 
  - "reflection"
  - "web-dev"
tags: 
  - "css"
  - "design"
  - "html"
  - "javascript"
  - "research"
  - "responsive"
  - "themes"
---

> “I may not have gone where I intended to go, but I think I have ended up where I needed to be.”  
> ― Douglas Adams (1989, p. 124)

So up until the 24th of December I dallied with solutions for the navigation, but I had not really tackled the core issue. It was truly the elephant in the room, as so much of the mobile responsiveness that I hoped for my site hinged on the navigation working smoothly. I spent quite a bit of time looking around the web for inspiration, usually finding elaborate JQuery scripted examples; much as I found with the search for sliders/carousels. I really wanted to build it myself and resolved to create with CSS and JavaScript.  
  
The bulk of my inspiration ended up coming from the NHS Choices website's navigation ([http://www.nhs.uk/pages/home.aspx](http://www.nhs.uk/pages/home.aspx)). It isn't responsive, but the styling of it says serious and health, so I thought what if I make a really responsive nav/menu based on a similar layout?  
I also really didn't want to create a hamburger menu (the three lined menu icon used on many mobile/responsive sites). Personally I think that these are overused and when I observe folks try to use them in day job, they often lead to frustration. This is particularly the case for those people who do not use the Internet on their phones/tablet that often (they might have a few favourite apps though) or those who are new to having a smart device. It was reassuring to find that I am not the only one who feels this way about the _burger_ ([Abreu, 2014](https://lmjabreu.com/post/why-and-how-to-avoid-hamburger-menus/); [Pernice & Budiu, 2016](https://www.nngroup.com/articles/hamburger-menus/)). So I decided to go with a simple button labelled menu which expands or contracts based on the media queries.  
To make this look nice I put in a bit of CSS animation smoothing for the transitions. Although I took inspiration from other folks coding (references are below and in the markup) the navigation is original. I decided that my button would trigger the header to become bigger or smaller based on an Active class in the CSS. I also had to figure out how to make the button toggle the active class (drew inspiration from this example for that: [http://codepen.io/razitazi/pen/WbZaOq](http://codepen.io/razitazi/pen/WbZaOq) <fn>I must add that I did not add the class effect to the <body> and they did. I added it to the elements, I tried both but working with the individual elements worked better for my menu.</fn>.  
I also had to the solve the problem of the someone opening the menu and leaving it open and then resizing the page in a responsive web browser. This would just make the site look a bit broken. This was fixed in the end with a media query, although I did try scripting a solution with an eventlistener looking for the window resizing, this added to the processing burden as it would fire too many times. I also tried restricting it by setting it to look at the status of the menu, but the media query with transitions in the CSS was more elegant and worked in major browsers on Mac and PC (Firefox 31+, Chrome, Safari, IE9).  
A couple of days later I made a return-to-top button, creating a new piece of script that used the smoothScroll function (mentioned in earlier posts). This allows folks viewing the site on a desktop or tablet to quickly return to the top of the page. This was inspired by a button on one of the [wordpress themes that I use in my work](http://blogs.brighton.ac.uk/elearningteam/), <fn>The button on this site ([http://blogs.brighton.ac.uk/elearningteam/](http://blogs.brighton.ac.uk/elearningteam/)) appears once you are halfway down the page. I didn't feel the need for quite as much animation so I kept my button a bit simpler.</fn> I always liked it and wanted to create my own. I decided to alter and reuse the same svg, as the Flickity navigation button arrows. It is nicely minimalist arrow and is also design consistent (and I should add so much better than the arrow that I designed - below). Also I checked whether the svg code could be [optimised further](http://petercollingridge.appspot.com/svg-optimiser) and it was already as good as it could get.  
`var anchor = document.querySelector( '#top' );  
var topBtn = document.querySelector('.return-top-button');  
var options = { speed: 700, easing: 'easeOutCubic' };`  
`topBtn.addEventListener('click', function() {  
smoothScroll.animateScroll( anchor, topBtn, options );  
}, false );`

[![Image of arrow svg attempt](images/arrow.png)](http://fionamacneill.co.uk/blog/2016/12/26/navigation/arrow/)

The arrow that failed to make the grade

### References

Abreu, L. (2014, May 14). Why and how to avoid hamburger menus - Louie A. - mobile UX design \[Blog post\]. Retrieved from [https://lmjabreu.com/post/why-and-how-to-avoid-hamburger-menus/](https://lmjabreu.com/post/why-and-how-to-avoid-hamburger-menus/)

Adams, D. (1989). _The long dark: Tea-time of the soul_ (8th ed.). London: Pan Macmillan.

Collingridge, P. SVG-Optimiser. Retrieved December 25, 2016, from [http://petercollingridge.appspot.com/svg-optimiser](http://petercollingridge.appspot.com/svg-optimiser)

Compete Themes. (2017). Tracks WordPress theme by compete themes. Retrieved January 4, 2017, from [https://www.competethemes.com/tracks/](https://www.competethemes.com/tracks/)

Flanagan, D. (2011). Handling Events. In _JavaScript: The definitive guide: Activate your web pages_ (6th ed.) (pp. 445–489). United States: O’Reilly Media, Inc, USA.

Kadlec, T. (2012). Media Queries. In _Implementing responsive design: Building sites for an anywhere, everywhere web_ (pp. 53–94). Berkeley, CA: New Riders Publishing.

LePage, P. (2017, January 9). What makes a good mobile site? Retrieved January 9, 2017, from [https://developers.google.com/web/fundamentals/getting-started/principles/](https://developers.google.com/web/fundamentals/getting-started/principles/)

Pernice, K., & Budiu, R. (2016, June 26). Hamburger menus and hidden navigation hurt UX metrics \[Blog post\]. Retrieved from [https://www.nngroup.com/articles/hamburger-menus/](https://www.nngroup.com/articles/hamburger-menus/)

Sherwin, K. (2015, June 7). Low-contrast text is not the answer \[Blog post\]. Retrieved from [https://www.nngroup.com/articles/low-contrast/](https://www.nngroup.com/articles/low-contrast/)
