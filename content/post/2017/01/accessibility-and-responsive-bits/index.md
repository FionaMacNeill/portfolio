---
title: "Accessibility and responsive bits"
date: "2017-01-02"
categories: 
  - "reflection"
  - "web-dev"
tags: 
  - "accessibility"
  - "compliance"
  - "css"
  - "design"
  - "images"
  - "portfolio"
  - "reflection"
  - "responsive"
coverImage: "Screen-Shot-2017-01-01-at-18.24.44.png"
---

This journal entry represents a mammoth effort to add high-quality content to the site.

1. **I developed and added the patient story.** This was based on a characteristics list which I worked through rather vigorously on the afternoon of the 25th. This is still in handwritten form, so I will link to it as a google doc later on. I have included some key references for that process below. I want to highlight the National Joint Registry (2016) data, which was particularly helpful during the process of defining the patient story. Also the specific images that I used will be cited on the portfolio site (including cc0 works; royalty-free works) as I feel it is always very important to include the provenance of images in any context, but especially when engaging in a thought process based on a fictional patient/nurse interaction.

2. **I added images to support the patient story.** These images were sourced from pixabay and one of my all-time faves, Creative Commons search as a means to filter Flickr images by license ([search.creativecommons.org](http://search.creativecommons.org/)).

3. **I recreated the images that I found for the patient story as drawings in Adobe Illustrator.** I wanted the images in the timeline to be small (100px x 100px); this is a limited amount of 'bandwidth' to communicate a visual concept. For this reason I decided to use Adobe Illustrator to trace the images and then re-paint them, so that I could accentuate certain aspects through the use of selective colour. This worked well and I did investigate whether these images could be included as svgs, but the visual information was too complex as they were based on photographic materials. As a result I stuck with .png format as the final output. ![svg version of image - less visual information](images/Screen-Shot-2017-01-01-at-18.24.28.png)] .svg version of a timeline image - quite a bit of artifacting (tech-speak for mess) in the image render and it looks too sketchy ![screenshot of the png version image](images/Screen-Shot-2017-01-01-at-18.24.44.png).png version of the same image in Adobe Illustrator - more of the visual information from the original photograph is retained. This version has the right level of abstraction.

4. **All of the images were optimised using [Kracken.io](https://kraken.io/).** Honestly, I absolutely love this tool and will be using this from now on for all my images. Their algorithm somehow trims off the excess while keeping the core visual information.<br>
5. **Accessibility.** I ran an accessibility analysis on the site using the WAVE Web Accessibility Tool ([http://wave.webaim.org/](http://wave.webaim.org/)). It is pretty good, I still have a few aria, alt and title tags to include here or there but I have made progress in this area.

6. **Infuriating.** As someone who uses Reader View (I found out that this is the official name for it) mode in Firefox and the equivalent in Safari, I was very frustrated by the restrictive and arbitrary local style sheet implemented by this mode. I have spent way too much time customising how the site looks in this context, but it really mattered to me as this would really put me off a site. Also, focusing on it has highlighted the importance of the semantic web; the _reader_ mode taps into the <sections> and other html5 element definitions. With a bit of hardcore tweaking, I finally have something that I can stand behind. The tweaking is outlined in [this development post](http://fionamacneill.co.uk/blog/2017/01/08/lots-of-changes-to-this-version-of-the-css/), however I found out by digging into the _reader_ displays in the respective browser stylesheets that they will ignore certain css classes. Specifically I needed to implement a class called .hidden which is the container for the flickity carousel dots. The 'dots' are completely useless in the _reader_ view and just look like an orphaned ordered list. I also instituted a .sr-only class which is applied to loading GIFs and other elements which should not be shown in the _reader_ mode. All of this digging will serve me well for the print stylesheet, no doubt...

7. **I ran the Google mobile accessibility test on the site - It passed!** Here is the proof: [https://search.google.com/search-console/mobile-friendly?id=W8x9QG2vBB-\_NxSwy4fVLQ](https://search.google.com/search-console/mobile-friendly?id=W8x9QG2vBB-_NxSwy4fVLQ) There is still a lot of content to add, but it is great to know that I am on the right track.

### References

BBC (2013, January 16). Going paperless “would save NHS billions.” BBC Health. Retrieved from [http://www.bbc.co.uk/news/health-21033984](http://www.bbc.co.uk/news/health-21033984)

BBC (2016, September 7). NHS: Health apps to inform patient records. BBC Health. Retrieved from [http://www.bbc.co.uk/news/health-37290126](http://www.bbc.co.uk/news/health-37290126)

Booth, R. (2016, December 13). The doctor on your Xbox? The NHS needs more digital ambition. The Guardian. Retrieved from [https://www.theguardian.com/healthcare-network/2016/dec/13/nhs-digital-tech-smartphones-jeremy-hunt](https://www.theguardian.com/healthcare-network/2016/dec/13/nhs-digital-tech-smartphones-jeremy-hunt) 

BS EN ISO 13485:2016 Medical devices. Quality management systems. Requirements for regulatory purposes. (2016). Retrieved 22 December 2016, from [https://bsol-bsigroup-com/Bibliographic/BibliographicInfoData/000000000030339592](https://bsol-bsigroup-com/Bibliographic/BibliographicInfoData/000000000030339592) 

BS ISO 13606-2:2008 Health informatics. Electronic health record communication. Archetype interchange specification. (2008). Retrieved 22 December 2016, from [https://bsol-bsigroup-com/Bibliographic/BibliographicInfoData/000000000030170710](https://bsol-bsigroup-com/Bibliographic/BibliographicInfoData/000000000030170710) 

Choices, N. (2016, November 1). Health and fitness trackers. Retrieved January 2, 2017, from [http://www.nhs.uk/Conditions/nhs-health-check/Pages/tools-and-technology-that-can-help.aspx](http://www.nhs.uk/Conditions/nhs-health-check/Pages/tools-and-technology-that-can-help.aspx) 

Dolatabadi, E., Babak, T., & Alex, M. (2014). Vision-based approach for long-term mobility monitoring: Single case study following total hip replacement. Journal of Rehabilitation Research and Development, 51(7), 1165–76. 

Farmer, A. Wearables sector grows as smartwatches increase in popularity. Retrieved January 2, 2017, from [https://yougov.co.uk/news/2016/03/18/wearables-sector-grows-smartwatches-increase-popul/](https://yougov.co.uk/news/2016/03/18/wearables-sector-grows-smartwatches-increase-popul/) 

Heartfield, R., Loukas, G., & Gan, D. (2016). You are probably not the weakest link: Towards practical prediction of susceptibility to semantic social engineering attacks. IEEE Access, 4, 6910–6928. doi:10.1109/access.2016.2616285 

Institute for Quality and Efficiency in Health Care (2014). What can help relieve anxiety before surgery? - PubMed health - national library of medicine - PubMed health. Retrieved from [https://www.ncbi.nlm.nih.gov/pubmedhealth/PMH0072741/?report=classic](https://www.ncbi.nlm.nih.gov/pubmedhealth/PMH0072741/?report=classic) 

Johansson Stark, Å., Charalambous, A., Istomina, N., Salanterä, S., Sigurdardottir, A. K., Sourtzi, P., … Bachrach-Lindström, M. (2016). The quality of recovery on discharge from hospital, a comparison between patients undergoing hip and knee replacement - a European study. Journal of Clinical Nursing, 25(17-18), 2489–2501. doi:10.1111/jocn.13278 

Nasr, N., & Enderby, P. (2014). Redefinition of life experience following total hip replacement: Analysis of narrative as performance. International Journal of Orthopaedic and Trauma Nursing, 18(2), 89–98. doi:10.1016/j.ijotn.2013.07.005 

National Information Board. (2015, March 4). National information board’s workstreams. Retrieved January 2, 2017, from [https://www.gov.uk/government/publications/national-information-boards-workstreams](https://www.gov.uk/government/publications/national-information-boards-workstreams) 

National Joint Registry. (2016). 13th Annual Report 2016 National Joint Registry for England, Wales, Northern Ireland and the Isle of Man Surgical data to 31 December 2015. Retrieved from [http://www.njrcentre.org.uk/njrcentre/Portals/0/Documents/England/Reports/13th%20Annual%20Report/07950%20NJR%20Annual%20Report%202016%20ONLINE%20REPORT.pdf](http://www.njrcentre.org.uk/njrcentre/Portals/0/Documents/England/Reports/13th%20Annual%20Report/07950%20NJR%20Annual%20Report%202016%20ONLINE%20REPORT.pdf) 

NHS Choices. (2015, November 3). Health Apps library - NHS choices. Retrieved January 2, 2017, from [http://www.nhs.uk/pages/healthappslibrary.aspx](http://www.nhs.uk/pages/healthappslibrary.aspx) 

Press Association (2016, September 7). NHS to have one website for appointments, prescriptions and advice. The Guardian. Retrieved from [https://www.theguardian.com/society/2016/sep/07/nhs-one-website-appointments-prescriptions-advice](https://www.theguardian.com/society/2016/sep/07/nhs-one-website-appointments-prescriptions-advice) 

Pulkkinen, M., Junttila, K., & Lindwall, L. (2015). The perioperative dialogue - a model of caring for the patient undergoing a hip or a knee replacement surgery under spinal anaesthesia. Scandinavian Journal of Caring Sciences, 30(1), 145–153. doi:10.1111/scs.12233 

Rudolfsson, G. (2013). Being altered by the unexpected: Understanding the perioperative patient’s experience: A case study. International Journal of Nursing Practice, 20(4), 433–437. doi:10.1111/ijn.12195 

Wilson, D. (2016). An overview of the application of Wearable technology to nursing practice. Nursing Forum. doi:10.1111/nuf.12177 

Wilson, C. J., Mitchelson, A. J., Tzeng, T. H., El-Othmani, M. M., Saleh, J., Vasdev, S., … Saleh, K. J. (2015). Caring for the surgically anxious patient: A review of the interventions and a guide to optimizing surgical outcomes. The American Journal of Surgery, 212(1), 151–159. doi:10.1016/j.amjsurg.2015.03.023 

Image source: "[Calendar days of the week](https://pixabay.com/en/calendar-days-day-of-the-week-487695/)" by [422737](https://pixabay.com/en/users/422737-422737/) is licensed under [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/deed.en)
