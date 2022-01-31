---
title: "Major discoveries, minor anguish"
date: "2015-12-21"
categories: 
  - "ux"
tags: 
  - "reflections"
  - "structure"
  - "ux"
---

You may ask, what happened to you Fiona, between 6/12 and 20/12? Well this is what happened. I was teaching an online course called the 12 Apps of Christmas (a satellite of course run at Regent's University, London) and it was ALL consuming. I was also working on my Learning Object project during this time (and you thought I was slacking!) however, for the most part I have to admit to reverting to paper reflections for a while, due to sheer convenience. Currently my notes are collectively living on bits of scrap-paper, serviettes/napkins, and Evernote entries. I plan to pull them together here over the next few days, a process that I have started with the inclusion of [my reflection of using a learning object as an end user](https://fionamacneill.co.uk/post/2015/12/real-time-reflection-experience-of-completing-a-learning-object/), I will include more on that later in the post. 

## First a few relevant reflections from my experience working on 12 Apps of Christmas

After the course we ran a completion survey. Although there is only a small number of responses so far (11 respondents out of 192 course subscribers; survey is open until the end of January), the responses do correlate with some of the observations that I had made. As the course was designed as an opportunity for academic staff, the insights into that population are helpful as I move forward with the Learning Object design, that is geared to the same community. _Course subscribers really appreciated clear image-based instructions with accompanying step-by-step written annotation._ Commentary: This could inform aspects of user documentation for the Learning Object. Specifically, the idea to include accompanying PDF guides for topics is supported by this anecdotal evidence. _Four learning activities or exercises is about the right number to minimise time and interest drop-off._ 

![screenshot of some of the results](images/Screen-Shot-2015-12-28-at-14.44.10-21v040u.png) 

### Commentary

We had a structure of 12+ exercises due to the preexisting structure of the 12 apps course, but interest did drop-off sharply after the 4th day (1 exercise per day). However, when considering a learning object this would seem like a pertinent observation. Also the topic of the learning object is probably (lets be honest) less interesting than learning about mobile apps presented with a festive theme. 

![Google Analytics for Dec 2015](images/Screen-Shot-2015-12-28-at-14.47.21-1pef2hw.png) 

> Beware of the inverse Field of Dreams (1989) effect...If you build it, they won't necessarily come



### Getting as much web traffic as we did took major effort

Building and maintaining the blog where we delivered the content; promoting the content via Twitter and keeping to our self-imposed publishing deadlines. In spite of this effort, the traffic dropped off after the 4th day, as documented in the screenshot from the site analytics above. 

I think that it is important to admit that learning resource content and therefore the Learning Object that I am designing has a very limited shelf-life, both in the sense of consumable shelf-life and continued relevance. This does not undermine the reusable goal of the Learning Object and it's Open Education ethos, but it does mean that it is more of a reusable template as opposed to being completely reusable in and of itself. I think that best way of considering the reuse aspect is that this Learning Object can be reused through a simple hyperlink to it, but is not geared towards being part of a open learning object repository (it would continue to live with the client university, university-x). Furthermore with my learning technologist hat on, driving traffic to the learning object would require a clearly structured publicity plan so that it was viewed as a timely tool in relation to the changes to DSA funding. 

Finally, this point really speaks to the importance of the delivery environment and how it portrays the importance of the Learning Object. As the Learning Object is academic staff-focused it is not best placed within the Virtual Learning Environment, a more centralised site with a focus on learning and teaching guidance at the fictional client university may be more appropriate. This will help to ensure that our main target audience have ready access and memorable access. So this is the spot in my thought process where I revised the purpose **sentence** slightly, as it wasn't quite right:

> Changes to funding for support of disabled students, necessitates the need to increase academic staff knowledge of best practices involving technology, to help disabled students and to fill areas of deficit created by the reduction of funding.

### The act of doing this resulted in a crucial thought...

This Learning Object is to promote awareness of DSA and accessible practices. How on earth did it end up being about Microsoft Word? I realised that by narrowing the scope, as my prior ideas were too expansive for the project prescribed by my instructor, I also undermined the purpose of the Learning Object. However, I was relieved to realise that this was largely a matter of semantics and learning content rather than an issue that would affect the "structure plane" (Garrett, 2011) of the Learning Object. 

To summarise, the Learning Object will still focus on accessibility in documents but this will be presented alongside information about DSA and increasing awareness of different student needs, so the new provisional title is: _Making your documents accessible._ The only aspects that still look at software-based techniques are the guidance PDFs and the _offline exercise,_ which are easier for university-x support staff to update independently and then add new versions to the Learning Object's back-end storage. 

Another thought that I had in relation to this point, is that learning video repositories like Lynda.com might be provided at university-x, so software training in my Learning Object would be a _poor relation_ when compared to the quality of such repositories. Therefore the key features that set the Learning Object apart are the bite-sized and context specific learning topics, the option to complete it anonymously and its enhanced accessibility. The Learning Object may also be more approachable for users who find the vast choice of videos that are available in a service like Lynda.com to be overwhelming as a starting point. 

## Other major discoveries

After I undertook [my reflection of using a learning object](https://fionamacneill.co.uk/post/2015/12/real-time-reflection-experience-of-completing-a-learning-object/), I decided to take a shot at [sketching some wireframes based on v5 of my UML model diagram](https://fionamacneill.co.uk/post/2015/12/bits-pieces-put-together-to-present-a-semblance-of-a-whole/). However, as soon as I started to do it my fears were realised and it became clear that I would need to revise the scenarios and then change the UML model diagram accordingly. This was a lot of extra work, but worth doing as it is important to me that I create something that hopefully equals or improves upon existing Learning Objects. 

Here is my first shot at sketching around about 20th of December: 

![wireframe sketches 1](images/featuredpost1-2b0dvmx.png) 

### As a result of this I decided to...

1. I removed one of the Topics, _Readability._ As it would be covered in _Fonts & Legibility_ and was redundant. It would also add to the time that it would take to complete the Learning Object and this cannot exceed 30mins (a usability requirement).
2. Removed _view feedback_ from the Topics as feedback is built into the proceedings of a learning activity - previously called _Quiz_ and then later _Lesson_ in the UML iterations.
3. Established the use of a learning activity, based "programmed instruction" as defined in the IMS Learning Design Specification (2003a, 2003b). This model features questions, presented alongside information; these will take the form of multiple choice questions with built-in feedback. This is based on an established design pattern outlined in the IMS LDS (2003b, Section 4.1, para. 1).
4. I have worked on standardising the language within the scenarios and Learning Object in the wake of what I have learned through study of the IMS Design Specification.
5. I added a centralised topic index page. I had something like this very early on, but it became clear to me after I worked though a Learning object myself that users need a clear overview of the contents of the learning object from the get-go. This also displays the test and certificate, although not available immediately, to give users an idea of the narrative flow of the proceedings as well as the internal end goal; obtaining the certificate.
6. I added a glossary as a global component of the Learning Object. This was based on a needs from the user characteristics that I had not picked up on for users external to university-x. I also felt frustrated by the lack of a glossary when I was using a Learning Object as a user.
7. I added settings and help as a global component of the Learning Object. This is based on the ideas from my [earlier post](https://fionamacneill.co.uk/post/2015/12/bits-pieces-put-together-to-present-a-semblance-of-a-whole/), when I felt that use of the accessibility settings needed to be built into the task scenarios.
8. Having quizzes for each topic, no longer made sense and as an incentivizing measure I added a central test that becomes available once the three main topics are completed.
9. The introduction became a _tutorial_ rather than _slides_. Slides were too visually prescriptive and I want to provide a step-by-step guide so that users can learn how to use the interface quickly.
10. Plus there is the glaringly obvious oversight... in addition to the normal objectives of software this Learning Object requires Learning Outcomes. **This is the reason why I am no longer referring to the Learning Object as LO, as this is a common shortening for Learning Outcomes in educational terminology and may lead to confusion.**
11. I took out task scenario 2 where the user could return to the saved Learning Object via a hyperlink in an email. This is not great practice as it encourages behaviour on the part of the user that could lead to them becoming victims of phishing in the future (Van Duyne, Landay, & Hong, p.555). The solution is to provide a clear link to a university domain parent page, rather than a user-specific URL and instruct the user to copy and paste the parent URL into the web browser address bar.

After all this, I ended up with the following - I feel MUCH more positive about this as the structure makes more sense. 

![The second iteration of the wireframe sketches](images/02wireframes-239sxt1.png "Half of this image is contrast-adjusted as it was drawn in pencil.") 

### A few notes about IMS LDS

I have mixed feelings about my discovery of the IMS Learning Design Specification. I came across it as I searched the ALT (Association of Learning Technologists) wiki, as I was curious what standards and specifications exist for Learning Technologies as these technologies have been around for a long time. Initially I came across information on Educational Modelling Language, which has folded into the IMS standard (original information from the ALT wiki which no longer exists as of 2022 when this post was revisited). 

On the one-hand the specifications feature learning design patterns, which are immensely valuable to this project and also within my day job. The specifications also include a very comprehensive outline of the XML metadata requirements that are needed to create a Learning Object that is truly reusable and also searchable; the following article some some good annotation of the XML to demonstrate the metadata properties (Ragbir & Mohan, 2009). However, as a specification it is too complex for this project, so as much as I would like to create a perfect learning object, in order to be compliant with the standard I would need to start from scratch and create something with multiple roles (student and support) and far more complex taxonomies. 

I also looked into whether I could adapt it and use it as a documentation standard, as a perhaps more appropriate alternative to the NASA documentation standard (1991), however as I started to map the necessary concepts over the contents page and it became clear that would not be possible within the scope of this project. 


![Trying to map to IMS standards](images/Screen-Shot-2015-12-28-at-11.49.00-1sps8rh.png "Trying to map the IMS Learning Design Information Model to my existing work and concepts that I need to cover. It didn't go well (screenshot from 2003a).")

### So what am I going to use from IMS LDS?

- I have tried my best to use the language outlined in the IMS LDS as this will provide a common way to describe the processes, architecture and learning design using terminology that is understood in my professional field.
- I will reference some of the learning design patterns (as found in Section 2. Use Cases in 2003b) as they are very helpful and provided some positive validation of the work that I had done so far, in terms of the structural make-up of a Learning Object.
- I absolutely love the stage-play metaphor that the IMS LDS standard uses to explain a learning object. In short a Unit of Learning (UoL), as defined in the standard, is a package that includes the learning content, including code and physical files alongside the specified metadata. This content is "played" and is compatible with different delivery "environments". The actions or method within the UoL are a series of "Plays". Those plays are structured as "acts" and within the acts the "Roles" perform their requisite "activities" within the "environment" (2003b, Section 3.2.3). The most succinct description of the standard that I have found is a PowerPoint presentation by researchers from the University of Vienna, Introduction to IMS Learning Design (Derntl, Neumann, & Oberhuemer, 2009).
- Having looked at the NASA software documentation standard (1991) again I felt that an adapted version of the IEEE Recommended Practice for Software Requirements Specifications (1998) will actually be more suitable in terms of outlining the final concept document. This standard has more common group with the IMS LDS.

As for the "minor anguish" of this post's title, as you can tell from the my writing above, discoveries have resulted in substantial work and with limited time available this has certainly led to a certain level of anguish. This was largely due to the need to back-track in certain areas. However, I now feel that I am almost back on-track, with the aim of completing my wireframes before the Christmas holiday is out. 

## References

Derntl, M., Neumann, S., & Oberhuemer, P. (2009). _Introduction to IMS Learning Design_ \[PowerPoint slides\]. Retrieved from http://www.slideshare.net/mikederntl/introduction-to-ims-learning-design 

Garrett, J. J. (2011). _The elements of user experience: User-centered design for the web and beyond_ (2nd ed.). Berkeley, CA: New Riders Publishing. 

Gordon, C., Gordon, L. (Producers), & Robinson, P. A. (Director). (1989). _Field of dreams_ \[Film\]. USA: Universal Pictures. Retrieved from http://www.imdb.com/title/tt0097351

IEEE. (1998). I_EEE Recommended Practice for Software Requirements Specifications_," (IEEE Std 830-1998). doi:10.1109/IEEESTD.1998.88286

IMS Global Learning Consortium. (2003a). _IMS learning design information model_ (Version 1.0). Retrieved from IMS Global Learning Consortium Online. 

IMS Global Learning Consortium. (2003b). _IMS learning design best practice and implementation guide_ (Version 1.0). Retrieved from IMS Global Learning Consortium Online. 

NASA-STD-2100-91. (1991). _NASA software documentation standard_. Retrieved 29 November 2015, from http://ntrs.nasa.gov 

Ragbir, D., & Mohan, P. (2009). Creating reusable lesson plans for e-learning using the IMS Learning Design specification. _International Journal of Education and Development using ICT_, _5_(4). Retrieved from [http://ijedict.dec.uwi.edu/viewarticle.php?id=852](http://ijedict.dec.uwi.edu/viewarticle.php?id=852) 

Van Duyne, D. K., Landay, J. A., & Hong, J. I. (2006). _The design of sites: Patterns for creating winning web sites (2nd edition)_ (2nd ed.). United States: Prentice Hall PTR.
