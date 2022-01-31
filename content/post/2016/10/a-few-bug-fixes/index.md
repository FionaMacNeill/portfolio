---
title: "A Few Bug Fixes"
date: "2016-10-21"
categories: 
  - "journal-dev"
tags: 
  - "accessibility"
  - "compliance"
  - "github"
  - "journal"
  - "label"
  - "reflection"
  - "themes"
---

I will write a longer post about the investigatory work that I have completed for my portfolio very soon. However in the meantime, I wanted to quickly outline some bug fixes in my child theme. Full details can be found in [my GitHub repository here](https://github.com/FionaMacNeill/learningjournal).

These changes were based on reports from the:

- W3C Markup Validation Service (W3C, 2016)
- IDI Web Accessibility Checker (AChecker, 2016)

## label

I finally managed to fix the label tag issue (mentioned in the ["contenders" section](http://fionamacneill.co.uk/blog/2016/10/13/theme-testing/#contenders) in my last post). It was missing the id, so once I added id = "search" into the php file and added <label for ="search" to the searchform.php file it was sorted. That took a bit of troubleshooting for sure.

## role

The NU HTML checker flagged some role distinctions that are not required for certain elements in HTML. I could tell that these roles were not needed in my updated child theme, so I removed the tags. These needed to be altered in the following files: header.php, index.php, sidebar.php and footer.php New versions of these files have all been added to both the child theme folder and my [GitHub repository](https://github.com/FionaMacNeill/learningjournal).

## footer

I got the footer displaying, not only my freshly minted WCAG 2.0 AA compliance badge[^1], but also my design credentials. Doesn't sound like a big thing, but it took me a while to figure out how to adapt the nested php "echoes" from the parent theme for my own purposes. More soon...I'll be working on wireframes this weekend.

#### References

AChecker. (2011). IDI web accessibility checker: Web accessibility checker. Retrieved October 21, 2016, from [AChecker website](http://achecker.ca/checker/index.php)

W3C. (2016). The W3C markup validation service. Retrieved October 21, 2016, from [https://validator.w3.org/](https://validator.w3.org/)

[^1]: I'll have to keep testing this periodically as things that you add to specific posts can prompt warning. It is a good way to ensure that I pay as much attention to the mark-up as I do to the written content of this journal.
