---
title: "Finishing touches - Eval pt 2"
date: "2017-01-23"
categories: 
  - "journal-dev"
  - "reflection"
  - "web-dev"
tags: 
  - "accessibility"
  - "compliance"
  - "css"
  - "github"
  - "journal"
  - "operation"
  - "portfolio"
  - "reflection"
  - "responsive"
  - "stakeholder"
  - "wearable"
  - "wordpress"
---

I want to take this opportunity to revisit the first goals of this Journal and also of the portfolio site and see what I have achieved. There are of course areas that I would have liked to do more with but I have kept them on my [Trello board](https://trello.com/b/4a20fYpf/web-development-portfolio-project) for future reference as the portfolio site particularly will live on.

## Goals for this journal

_"The posts in this journal will follow two reflective threads as I work through the module. The first thread is the development of this journal site, based on an independent install of the WordPress Content Management System or CMS (2016). I will outline my thinking behind decisions that I have take related to customisation and in particular accessibility and mobile responsiveness. These are the two key areas that I would like to learn more about during the module."_ \-Yes, I believe that I have done this. _"...The second thread is related to the creation of my portfolio website. This part of the coursework will be coded from scratch and needs to rich in features, structurally sound and accessible."_ \- Yes, I have done this although it has been a very long road. _"It is important to me that this journal’s theme is as accessible as possible,...."_ - Tried my best on this, although I would have liked to do more with the visited links and some of the buttons. _"...based on the WordPress theme templates available. At some point down the line I may even create a child-theme in order to customise it to the necessary level. For this reason I need to spend a bit of time checking the coding integrity of some of the themes that I have installed to ensure that they are suitable for customisation."_ \- I did this and this site is proudly running a child theme. _"...I have installed a list of themes filtered for accessibility features. Please bear with me, as in these early days, it is likely that this site might change it’s skin a couple of times while I decide on a suitable theme. I will also conduct some more thorough investigations using a local copy of WordPress and themes in MAMP (appsolute GmbH, 2016)." -_ I did this and also created a connection to my GitHub profile via Cybersyn plugin and setting up a RSS from my Atom feed. I also provided options for user customisation through the use of the [stylesheet switcher](http://fionamacneill.co.uk/blog/2016/10/31/development-prototypes/) and the accessibility plugin.

### Goals for the portfolio site

### Original Concept with annotation (areas achieved are highlighted in blue)

The project’s working title is _p__atient pre-op anxiety infographic._ It is a website structured around a central page, which leads the viewer through a fictional narrative of a patient’s experience of anxiety while awaiting a medical operation or procedure. In the narrative the patient will be using an electronic wearable device to track their own vital signs and also for logging their anxiety levels – the influence of this countermeasure will be explored. The narrative is represented through a navigable timeline enriched with the use of graphical, written and statistical information. The underlying project, to use wearable devices to measure patient pre-operative anxiety is attributed to and courtesy of Dr. Theofanis Fotis (School of Health Sciences, University of Brighton), whom I am collaborating with at this time. **Scope** The _p__atient pre-op anxiety infographic_ will:

- deliver an approachable overview of a research project – the proposed research project is to design a user interface for a medical wearable device to measure anxiety;
- explain the issues that can result from pre-operative stress in patients;
- provide a point of entry for those with little or no knowledge of the subject as well as explain the potential benefits of the project to experienced medical professionals.

The _p__atient pre-op anxiety infographic_ will not:

- provide in-depth medical information;
- provide any fully formed solutions or recommendations for implementation of wearable devices in a medical setting;
- provide advice or suggestions for the production of patient care plans. As a narrative scenario it is exploring a hypothetical scenario in which a wearable device is used.

**Benefits** The _p__atient pre-op anxiety infographic_ will provide the following benefits:

- it will provide a valuable resource for explaining the research project to potential funders and future stakeholders; - _Hopefully in the future_
- it will help to raise awareness of the potential issues related to patient pre-operative anxiety; _\- Hopefully if it finds a wider audience_
- it will highlight potential ways that increased knowledge of a patient’s vital signs and self-reported anxiety could improve patient care;
- it will provide an accompanying contextual information for the proposed future interface design project; _\- I have shifted my thinking it is more of a service design project._
- it will be a publicity tool, that can be used to explain the project within the academic and medical online communities. _\- Hopefully, again if it finds a wider audience._

**Goals** The following goals are related to the successful creation of the _p__atient pre-op anxiety infographic:_

- provide a valuable portfolio piece, not only in terms of web development, but also as a tool for the research team and collaborators;
- contribute to the approval and ethics approval of this as a concept for F.MacNeill’s final graduating project; _\- Hopefully, I am about to start writing this._
- stimulate dialogue around the issues and ideas raised by the _p__atient pre-op anxiety infographic; - Hmmm, this may have been a bit ambitious_
- encourage potential funders and stakeholders to invest in the project. _\- Hopefully..._

**Objectives**

- Create an accurate portrayal of a possible patient care scenario.
- Provide information highlighting the benefits of the proposed project.
- Pose the project concept as an open question in order to gauge feedback and interest from the medical community and potential funders and/or stakeholders.
- The user audiences for this are diverse but have one thing in common, they have very limited time to engage with a website of this kind. This website should take no longer than 10-15mins to navigate, the equivalent of a typical coffee/tea break. _\- I have hopefully achieved this_
- To be shared via social media between interested parties. _\- Did not get an opportunity to integrate any sharing tools._
- To be adaptive and easily viewed and navigated on mobile devices.
- To be accessible to those on older web browsers (as far as possible).
- To be accessible to users with disabilities, allowing for personal customisation (as far as possible). _\- The customisation wasn't really possible in the end._

To summarise, I believe that I succeeded in my goals to learn about web development, accessibility and to gain domain knowledge about the perioperative environment in preparation for my future project. http://fionamacneill.co.uk/blog/key-resources/

### Here is a quick list of the final finishing touches that I made to my site.

**Revisiting the post about my last meeting with the stakeholder** - ["I add some data to support this section"](http://fionamacneill.co.uk/blog/2017/01/12/final-meeting-with-stakeholder/) I added a google charts treemap to support the care section (Google, 2016). Using this as a way to show the comparative percentages between each of the different reasons. I wrote tooltips for the treemap to help with the navigation of the data I had to use html codes to make it work. **I added columns to the reference section** (Coyier, 2010). However, I also found that the reference section was too long and ended up moving the section to a new page for those viewing from mobile devices. When I develop the site further, I will probably always keep a link to a separate page as NHS trusts frequently block pages which link to external websites. I might be able to get a university domain cleared for their whitelist though. **I added the icons for the goals**. These were obtained from the Noun project and are cited on my new [Resource page](http://fionamacneill.co.uk/blog/key-resources/) which links up a lot of the artefacts which I have created as I have gone along. **I passed the mobile test and the validator tests**. Although, the Nu Html Checker (validator.w3.org) took the opportunity to yell at me about the aria tags/elements: [https://validator.w3.org/nu/?doc=http%3A%2F%2Fitsuite.it.brighton.ac.uk%2Ffjm19%2Fwearable%2F](https://validator.w3.org/nu/?doc=http%3A%2F%2Fitsuite.it.brighton.ac.uk%2Ffjm19%2Fwearable%2F)I tweaked them a bit, but decided to leave them as I had added them based on the results that I was getting from the screenreader. Mobile test: https://search.google.com/search-console/mobile-friendly?id=4uQnwXr\_vs07ixrqbFArEA **The print stylesheet was very tricky**. I ended up having to omit the timeline in the end as there was no way to format it in context. I found some really good articles via Smashing Magazine in the process of getting it sorted though. **Media queries for tablet devices.** I found some really helpful media queries on CSS-Tricks for this. Although the screen resolution in the queries was no longer compliant, so I had to remove that. This was important as I wanted to omit the tooltip and the keyboard navigation in from being seen on tablets. Based on experience iPads and Google Nexus (Nexi?) are the most used devices amongst the academic audience for the site. **Refresh button for data visualisations.** I found an onclick command (Lobito, 2015) for refreshing the web browser and I added this as a button. What had annoyed me was that everytime you resized the browser, the visualisations did resize, but they didn't update. This allows the user to refresh their view of the data. **Minify used to minimise CSS and JavaScript for the final production site files.** **I realised that I did have a lot of content sections rather than articles.** I had misunderstood some aspects of the structure and realised that I needed to revisit the guidelines on this.

#### References

Andrew, R. (2015, January 7). Designing for print with CSS – smashing magazine \[Blog post\]. Retrieved from [https://www.smashingmagazine.com/2015/01/designing-for-print-with-css/](https://www.smashingmagazine.com/2015/01/designing-for-print-with-css/)

ASCII. HTML codes - table of ascii characters and symbols. Retrieved January 19, 2017, from ASCII website: [http://www.ascii.cl/htmlcodes.htm](http://www.ascii.cl/htmlcodes.htm)

Coyier, C. (2010, November 5). Multiple columns \[Blog post\]. Retrieved from [https://css-tricks.com/snippets/css/multiple-columns/](https://css-tricks.com/snippets/css/multiple-columns/)

Coyier, C. (2016, July 23). Media queries for standard devices \[Blog post\]. Retrieved from [https://css-tricks.com/snippets/css/media-queries-for-standard-devices/](https://css-tricks.com/snippets/css/media-queries-for-standard-devices/)

Google. (2016, July 14). Treemaps. Retrieved January 19, 2017, from Google Charts website, [https://developers.google.com/chart/interactive/docs/gallery/treemap](https://developers.google.com/chart/interactive/docs/gallery/treemap)

Krammer, C. (2011, November 24). How to set up A print style sheet – smashing magazine \[Blog post\]. Retrieved from [https://www.smashingmagazine.com/2011/11/how-to-set-up-a-print-style-sheet/](https://www.smashingmagazine.com/2011/11/how-to-set-up-a-print-style-sheet/)

Lobito, P. (2015). Re: Button that refesh page on click. StackOverflow website. Retrieved 23 January 2017, from [http://stackoverflow.com/questions/29884654/button-that-refresh-page-on-click](http://stackoverflow.com/questions/29884654/button-that-refresh-page-on-click)

Mozilla Developer Network. (2016a, November 5). Using HTML sections and outlines. Retrieved January 23, 2017, from Mozilla Developer Network website, [https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/Using\_HTML\_sections\_and\_outlines](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/Using_HTML_sections_and_outlines)

Mozilla Developer Network. (2016b, November 28). Scale(). Retrieved January 23, 2017, from Mozilla Developer Network website, [https://developer.mozilla.org/en-US/docs/Web/CSS/transform-function/scale](https://developer.mozilla.org/en-US/docs/Web/CSS/transform-function/scale)

Mozilla Developer Network. (2017, January 1)."<article>". Retrieved January 23, 2017, from Mozilla Developer Network website, [https://developer.mozilla.org/en-US/docs/Web/HTML/Element/article](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/article)

Mullie, M. (n.d.) JavaScript and CSS minifier \[Computer software\]. Retrieved from [http://www.minifier.org/](http://www.minifier.org/)

Storey, D. (2013, March 8). Tips and tricks for print style sheets – smashing magazine \[Blog post\]. Retrieved from [https://www.smashingmagazine.com/2013/03/tips-and-tricks-for-print-style-sheets/](https://www.smashingmagazine.com/2013/03/tips-and-tricks-for-print-style-sheets/)
