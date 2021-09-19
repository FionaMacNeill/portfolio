---
title: "Wireframes 2+"
date: "2016-11-20"
categories: 
  - "web-dev"
tags: 
  - "css"
  - "design"
  - "wireframe"
---

This post displays iterations of wireframe 2. In this wireframe, I took ideas from wireframes 0 and 1, but removed the next buttons in favour of a timeline at the top of the page. The top section of the page, containing the timeline, is shown as overflow (beyond the width) of the page to indicate the dynamic content. Clicking on the _years_, and circles on the timeline is intended to swap out the slide content and information in the centre of the timeline section. The arrow buttons on the left and right were also intended to switch between the content slides. These buttons ideally would also be operable via arrow keys on the keyboard. \[caption id="attachment\_186" align="alignnone" width="840"\][![Image of wireframe version 2 ](images/wireframe2noguide-1024x1024.png)](http://fionamacneill.co.uk/blog/2016/11/20/wireframes-2/wireframe2noguide/) Version 1 - the top timeline is shown double-width in order to indicate the movement of the information.\[/caption\] \[caption id="attachment\_187" align="alignnone" width="840"\][![Image of wireframe 2 with anxiety levels visualisation shown](images/wireframe2withwave-1024x1024.png)](http://fionamacneill.co.uk/blog/2016/11/20/wireframes-2/wireframe2withwave/) Version 2: this version of the felt too blue - although I did like the way that the anxiety levels traversed the sections linking them together\[/caption\] \[caption id="attachment\_188" align="alignnone" width="840"\][![Image of wireframe 2 with two versions of the anxiety levels displayed](images/wireframe2_5DoubleWave-1024x1024.png)](http://fionamacneill.co.uk/blog/2016/11/20/wireframes-2/wireframe2_5doublewave/) Version 3: similar idea except this wireframe includes the colourful anxiety levels visualisation under the timeline. This works better as the anxiety levels directly relate the the narrative. If the anxiety levels under the timeline could be animated to appear as the timeline is navigated that would look great. I'll have to think about how best to do that (CSS3 I think).\[/caption\] \[caption id="attachment\_189" align="alignnone" width="840"\][![Image of wireframe 2 with two layers of levels](images/wireframe2withcolourwave-1024x1024.png)](http://fionamacneill.co.uk/blog/2016/11/20/wireframes-2/wireframe2withcolourwave/) Version 4 - this wireframe shows both versions of Anxiety levels (they look more like waves!) overlaid. It is a bit busy.\[/caption\] The new iteration of the design seemed cleaner and more focused in the sense that any page visitor would be immediately be shown the patient's story as an interactive narrative. However, this also meant that all my prior work on the smooth scrolling was for naught. I did try to see if I could tweak it to go from left-to-right or rather back and forth, but that was a futile effort. A related attempt at this was to look at transition whether I could build the timeline itself in CSS by creating a <div> for the line itself and a <div> for the timeline circles but adding them as squares and then using the border-radius at 100% made them into circle. As you can see from the video below, this is ended in a vomit-inducing interface. 

<iframe src="https://www.youtube-nocookie.com/embed/G0GsablXPlk?rel=0&amp;showinfo=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe>

Don't get me started on how dreadful this looked when I looked at it on my phone. \[caption id="attachment\_191" align="alignnone" width="230"\][![Image showing the mockup on a phone sized screen](images/mobileFAIL.png)](http://fionamacneill.co.uk/blog/2016/11/20/wireframes-2/mobilefail/) Mobile responsive fail\[/caption\] Further to this as I was influenced by the DuckDuck About page's interactive timeline (Titlow, 2014) I recreated it locally on mydevelopment computer. I then added it to my web space using the source files - stripping all that I could until it was only the timeline. However, I discovered that the coding and structure was not idea for this project. The code (CSS and Javascript particularly) had a lot of vague naming making it hard to follow and there was a LOT to strip out. So, the search for a solution continues, I think that I need to take a different approach to this problem...

### Considering colour

Upon looking at a number of medical websites for journals, professional bodies and organisations including:

- [NHS choices](http://www.nhs.uk/pages/home.aspx) (blue/orange/green)
- [Nursing and Midwifery Council](https://www.nmc.org.uk/) (dark blue, aquamarine, pink and lavender purple)
- [Royal College of Midwives](https://www.rcm.org.uk/) (dark blue, two hues of light blue, white, purple and grey)
- [Nursing Times](http://www.nursingtimes.net/) (dark blue, aquamarine and white)
- [Nursing Standard](http://journals.rcni.com/journal/ns) (scrubs green, two hues of dark blue, grey and orange for callouts)
- [The Lancet](http://www.thelancet.com/journals/lancet/issue/current) (purple, blue, green - a lot of white space)
- [Médecins Sans Frontieres](http://www.msf.org/) (red and black<fn>An outlier with the red and black theme, however this would underline the critical nature of the work they do providing aid in emergency situations.</fn>)
- [The British Medical Journal](http://www.bmj.com/thebmj) (blue and white, orange callouts)

The colour schemes contain a lot of blue and this influenced me to look at some different colour combinations. I used the palletton colour selector web application ([http://paletton.com/](http://paletton.com/)) to try a few bold colour combinations. I also tried it with some vision simulations (available on the bottom right) to see how the contrast behaved for different types of colour blindness. The swatches below show one of the better combinations I came up with, although it still needs work. \[caption id="attachment\_190" align="alignnone" width="400"\][![Image showing a colour scheme created using paletton](images/01palettonswatches.jpg)](http://fionamacneill.co.uk/blog/2016/11/20/wireframes-2/01palettonswatches/) Paletton colour scheme 1\[/caption\] The challenge with this medical site is that I feel I need to avoid a number of colours that may evoke negative associations. For example, hues of red might suggest blood and certain hues of yellow should be avoided due to the _hospital-yellow_ association. The blues above seemed a bit dark, so I tried some lighter hues for Wireframe 2, paying attention to the contrast between the text colour and the background colour.

### References

These are resources that I referred to beyond what I have linked to in the content above.

Border-radius. (2016, November 13). Retrieved November 27, 2016, from [https://developer.mozilla.org/en-US/docs/Web/CSS/border-radius](https://developer.mozilla.org/en-US/docs/Web/CSS/border-radius)

Crockford, D. (2008). Functions. In _JavaScript: The good parts: Working with the shallow grain of JavaScript_(pp. 26–45). United States: O’Reilly Media, Inc, USA.

Titlow, J. P. (2014, February 20). About DuckDuckGo. Retrieved November 19, 2016, from [https://duckduckgo.com/about](https://duckduckgo.com/about)
