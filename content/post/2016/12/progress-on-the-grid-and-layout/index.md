---
title: "Progress on the grid and layout"
date: "2016-12-08"
categories: 
  - "reflection"
  - "web-dev"
tags: 
  - "animation"
  - "compliance"
  - "css"
  - "design"
  - "javascript"
  - "performance"
  - "portfolio"
  - "reflection"
---

This week I completed some major fix-up on my grid. Remember when I thought that it was almost fixed? Well I was wrong. In fact I ended up recalculating the whole thing and basing it on a single column being 65px or 6.5% in width. Happily it is now working exactly as I need it to (Mozilla Developer Network saved the day again<fn>[https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS\_layout/Grids#Creating\_a\_fluid\_grid](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Grids#Creating_a_fluid_grid)</fn> - I am going to up my donation this year).

### I am feeling griddy

Now that my grid is in situ, I am able to base layout elements on  it. I do think that in most cases I will need to make unique versions of the columns and tweak the row layout, but keeping the grid architecture in place and temporarily adding the rows/columns to the html has been really helpful for planning out the sections (as shown in the screenshot below). I used my grid to start planning the layout of the content on the Flickity carousel cells - as it turns out this took quite a bit of work (more on that in my next post). I also had my first go at creating an SVG, albeit a very simple one as a placeholder for the first cell in the carousel. The SVG shows the outline of a head and I made it in Adobe Illustrator, this will need to be replaced by more of a photographic image for needs of the project.

### about-About

Adding in an _About_ section as the timeline really jumps right into talking about the fictional _Patient_. I will need to update the [task list](https://docs.google.com/document/d/e/2PACX-1vQNj8SiUKWqBOTRTo5rnLcG8NxToeAJ7B9Q1eWWRDdl-_Z-dCbCG-E8xzjOhSWc86TWtNntOcL7K84F/pub) to reflect this, but it remains within the bounds of the tasks as task scenario 1 included, "Read introductory information", this needs to become task scenario 2 and the others need to be bumped up. I also need to revise things where they are _areas_ as opposed to pages, it is bit too specific at the moment.

### Testing in Internet Explorer 9

I was astounded to find that pretty much everything on the site is working as one would expect in Internet Explorer 9. This is fantastic and vindicates some of the script selections that I have made in terms of browser support. I was very concerned that the z-index settings would not be respected, but thus far it is looking good. Safari is still a problem though... \[caption id="attachment\_233" align="alignleft" width="840"\][![Screenshot of the site on 9/12](images/journalimage81216-1024x575.png)](http://fionamacneill.co.uk/blog/2016/12/08/progress-on-the-grid-and-layout/journalimage81216/) Screenshot of the site on 9/12 shown side-by-side in IE9 and Chrome. I am now kicking my myself for not recording the exact browser version numbers on the PC I was using at the time! The majority of my day-to-day testing takes place on a variety of Mac, so I have to check on Windows whenever the opportunity presents.\[/caption\]

### Toying with the notion of animation

One of the sites that I have mentioned before, [gamification+](https://gamificationplus.uk/) has some pretty gorgeous and playful animations on it. I took a look through the code and the javascript attributes and most of it is managed via CSS. This is good, although I would am concerned about browser support and also performance rendering. As a consequence I probably won't add these features. As a pre-check I used the Chrome timeline tool to record the processes on an older computer that I have at home and I felt that the impact on performance would be a problem <fn>the new features operate at the limits of what I want, timing-wise so I will need to see if I can optimise them further. I have already removed aspects of the code that is not used.</fn>.

### References

Basques, K. (2016, December 8). How to use the Timeline tool. Retrieved December 8, 2016, from [https://developers.google.com/web/tools/chrome-devtools/evaluate-performance/timeline-tool](https://developers.google.com/web/tools/chrome-devtools/evaluate-performance/timeline-tool) Common CSS questions. (2015, October 26). Retrieved December 8, 2016, from [https://developer.mozilla.org/en-US/docs/Web/CSS/Common\_CSS\_Questions](https://developer.mozilla.org/en-US/docs/Web/CSS/Common_CSS_Questions) daneden. (2016, September 27). Daneden/animate.Css. Retrieved December 8, 2016, from [https://github.com/daneden/animate.css](https://github.com/daneden/animate.css) Grids. (2016, October 7). Retrieved December 8, 2016, from [https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS\_layout/Grids#Creating\_a\_fluid\_grid](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Grids#Creating_a_fluid_grid) Lewis, P. (2016, December 8). Rendering performance. Retrieved December 8, 2016, from [https://developers.google.com/web/fundamentals/performance/rendering/](https://developers.google.com/web/fundamentals/performance/rendering/) SVG and CSS. (2016, January 2). Retrieved December 8, 2016, from [https://developer.mozilla.org/en-US/docs/Web/Guide/CSS/Getting\_started/SVG\_and\_CSS](https://developer.mozilla.org/en-US/docs/Web/Guide/CSS/Getting_started/SVG_and_CSS) Z-index. (2016, December 2). Retrieved December 8, 2016, from [https://developer.mozilla.org/en-US/docs/Web/CSS/z-index](https://developer.mozilla.org/en-US/docs/Web/CSS/z-index)
