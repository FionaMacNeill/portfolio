---
title: "Building the grid"
date: "2016-11-22"
categories: 
  - "reflection"
  - "web-dev"
tags: 
  - "accessibility"
  - "css"
  - "design"
  - "responsive"
  - "wireframe"
---

After starting my initial experiments/prototypes for the portfolio project from a boilerplate I decided that I wanted to build my own responsive CSS grid from scratch. The grid turned out fairly well although there are some very slight issues with the column alignment which I need to sort out. I also still need to add the mobile device break points. I did find it very helpful to make use of the CSS calc() function to actively resize widths in percentages based on window size (calc()., 2016). This is a fantastic function although the support for it isn't universal yet (82.73 according to caniuse.com). Having said that I did try my grid in Safari to see how it behaved in an unsupported browser and I was pleased with how well it resized. \[caption id="attachment\_200" align="alignnone" width="919"\][![Screenshot showing the issue with column alignment](images/gridalignissue.png)](http://fionamacneill.co.uk/blog/2016/11/22/building-the-grid/gridalignissue/) The coloured overlay is included to highlight the issue with the column alignment.\[/caption\] \[caption id="attachment\_202" align="alignnone" width="613"\][![Screenshot showing the grid system with a photoshop grid/guides overlaid](images/fixthegridalignissue.png)](http://fionamacneill.co.uk/blog/2016/11/22/building-the-grid/fixthegridalignissue/) I will attempt to use the power of Photoshop to fix my mathematics - here is a newly sized grid overlay using Photoshop guides to figure out the correct calculations.\[/caption\] Just putting these calculations here for future reference. **Columns:** Columns = 12 Gutter = 15px **Rows:** Rows = 12 Gutter = 15px **Margins:** Top = 10px Left = 20px Bottom = 10px Right = 20px

### References

Calc(). (2016, May 17). Retrieved November 22, 2016, from [https://developer.mozilla.org/en-US/docs/Web/CSS/calc](https://developer.mozilla.org/en-US/docs/Web/CSS/calc)

Can I use... Support tables for HTML5, CSS3, etc. (2016, October 23). Retrieved November 27, 2016, from [http://caniuse.com/#search=calc](http://caniuse.com/#search=calc)

Drewniak, J. (2014, November 6). Creating your own CSS grid system. Retrieved November 25, 2016, from [http://j4n.co/blog/Creating-your-own-css-grid-system](http://j4n.co/blog/Creating-your-own-css-grid-system)

Gamache, D. (2016) A dead simple, responsive boilerplate. Retrieved November 25, 2016, from [http://getskeleton.com/](http://getskeleton.com/)

Imling, M. (2016). One% CSS Grid. Retrieved November 25, 2016, from [http://onepcssgrid.mattimling.com/](http://onepcssgrid.mattimling.com/)

Rand-Hendriksen, M. (2015, July 16). Making sense of the CSS box model. Retrieved November 25, 2016, from [https://www.lynda.com/CSS-tutorials/Making-Sense-CSS-Box-Model/372544-2.html](https://www.lynda.com/CSS-tutorials/Making-Sense-CSS-Box-Model/372544-2.html)

H5bp/html5-boilerplate. (2016, November 17). Retrieved November 25, 2016, from [https://github.com/h5bp/html5-boilerplate](https://github.com/h5bp/html5-boilerplate)
