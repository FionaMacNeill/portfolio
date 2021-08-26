---
title: Wearable for Health (2017-18)
summary: Smartwatches and smartphones to support surgery
tags:
- Research
date: "2021-07-16T00:00:00Z"
type: "book"

image:
  caption: "System Map for Apple Health created by Fiona MacNeill"
  focal_point: "Center"
  preview_only: true
  alt_text: System map diagram shows the relationship between Apple devices, APIs and Electronic Health Records. Caption in post includes further description.

gallery_item:
- album: wfh-survey
  image: devicebyage.png
  caption: Image 1 - Smartwatch brand distribution by age group as a bar chart.
- album: wfh-survey
  image: opplandhealth.png
  caption: Image 2 - Opportunity Landscape plot featuring diagonal lines to show sectors of opportunity.
- album: wfh-persona
  image: 01val-lucas-hip-replacement-sml.jpg
  caption: Image 3 - Persona for patient having a hip replacement. PDF version provided for detail.
- album: wfh-persona
  image: 02gemma-jarrett-cs-sml.jpg
  caption: Image 4 - Persona for patient having a caesarian section. PDF version provided for detail.
- album: wfh-recommendations
  image: 01rec-stack.jpeg
  caption: Image 5 - Reporting stack for patients. Text below image provides detail.
- album: wfh-recommendations
  image: 02rec-stack.jpeg
  caption: Image 6 - Reporting stack for frontline staff and consultants. Text below image provides detail.
- album: wfh-recommendations
  image: 03rec-stack.jpeg
  caption: Image 7 - Reporting stack for warehouse and auditing. Text below image provides detail.

# Optional external URL for project (replaces project detail page).
external_link: ""

links:
url_code: ""
url_pdf: ""
url_slides: "https://www.slideshare.net/secret/NeYLnmZbjtYGDY"
url_video: "https://youtu.be/2wM95lubobM"

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

## Introduction
This UX research project explored the use of information from patient-owned smartwatches and smartphones to support patient care prior to surgery. The project also assessed the informational needs of healthcare professionals, asking what data sources they would need from patient-owned smartwatches and smartphones to support care. Through the project research, I identified improvements which were later added to Apple WatchOS and Apple Health for iPhone. These included separating walking and running data, automatically detecting workouts, and providing relational data such as walking distance per day.

<p class="gallery-custom-caption"><a href ="https://lucid.app/documents/view/7a5f0dd2-3e17-45cc-b81c-4dee3d6b8cc9" target="_blank" title="LucidChart opens in new tab/window">Completed Service Blueprint can be viewed at LucidChart.</a></p>

![Iterative development of the Service Blueprint diagram presented in a chronological list](blueprint_iterations.png "Overview of the iterative development of the Service Blueprint used with participants as a means to understand and discuss a patient's journey. The printed version of the Service Blueprint is over two metres wide and is designed to be viewed as a long poster. It was created using LucidChart.")

## Client
A healthcare trust, cannot be named due to restrictions related to HRA ethical approval.

## Background
While completing an MSc in 2018 I used my dissertation project as an opportunity to explore a real-world area of UX research, wearable devices in digital health. The project focused on healthcare professionals as a user group to ascertain if the information from these devices was fit for purpose prior to creation of apps and software. The research was ethically approved and field work was completed in a clinical setting. The project took place over 6-months.
![System map for Apple Health, with devices and infrastructure. Caption includes description.](applehealthapp-system.jpg "The Apple Health app ecosystem is reliant on infrastructure provided by a healthcare provider. Inspired by ‘system maps’ in Stickdorn *et al.* (2018), This is Service Design Doing, pp. 58-63. Created using Adobe Illustrator CC as part of a competitor analysis. </br></br> Dotted lines indicate two-way data exchange and read/write relationship.</br> P ~ Patient, and HCPs ~ Healthcare Professionals.")


## Objective
To use the problem statement below, as the basis for an in-depth speculative UX research study to be written up as a dissertation and disseminated back to the UX and healthcare communities.

### Problem Statement
*Could information from patient-owned smartwatches and smartphones be used to support perioperative[^1] care?* 

[^1]: *Perioperative* ~ Encompasses the period prior to surgery, during surgery and through to the conclusion of recovery at home; as defined by the Royal College of Anaesthetists (RCoA, 2014, pp. 4-5).

## Roles, Methods, and Tools
I was the main researcher. My work was overseen by two supervisors: one supervisor was from a UX/academic background (named principal investigator), and one from a medical practice background, whom I brought on board through my own initiative.

### Highlighted methods
<ul>
    <li><a href="#interviews">Interviews</a></li>
    <li><a href="#survey-of-smartwatch-owners">Survey and Quantitative Analysis</a></li>
    <li><a href="#personas-and-low-fidelity-prototypes">Personae</a></li>
</ul>

### Interviews
In preparation for field work, I arranged interviews with professional contacts whom had relevant healthcare experience. I co-created a Service Blueprint diagram with these participants, outlining the patient journey. I also created a glossary, based on the qualitative data from interviews. This was to ensure that descriptive terms used in the recruitment materials, oral presentations, and dissertation were contextually accurate and appropriate.

Alongside this I formed a research collaboration with a healthcare professional working in a relevant role in practice. My collaborator helped to facilitate contextual interviews with healthcare professionals working in a clinical setting. These interviews were used as the basis for discovering data/information requirements. Second interviews were completed with the same participants. I used a lightweight card sorting exercise in the first interviews to allow participants to indicate, which types of health information were pertinent, and the order of importance (from most important to least important).

![Interview kit on a table, with do not disturb sign, pens, post-its, and a card sorting exercise'](research-wearable-for-health.jpg "Lightweight interview kit. Designed to be taken to a room in a clinical practice location and quickly picked up if needsbe. Cards were based on the core information types available from a smartwatch/smartphone, e.g., heart rate, exercise time, step count, etc. Cards created using Adobe Illustrator CC.")

### Survey of Smartwatch owners
I designed a survey, to gauge the attitudes of current smartwatch owners in relation to use of devices for health-related purposes. The survey was distributed via online user communities, social media, and targeted emails. The quantitative findings were presented in the dissertation and used to inform the list and prioritisation of requirements. The open-text responses were used to support human-factors analysis, looking at the likelihood of technology adoption and potential risks.

{{< gallery album="wfh-survey" >}}


<p class="gallery-custom-caption"><strong>Gallery Image 1</strong> - 75 survey respondents. A key observation is that the 45-54 age group holds the second highest proportion of ownership. These users will be entering the age-based demographics for procedures such as joint replacement over the next 12-20 years. Plotted using RStudio and ggplot2 (Wickham, 2016). Original data is included in <a href="#table-1">Table 1</a> in the <a href="#data">Data section</a>.</p>
<p class="gallery-custom-caption"><strong>Gallery Image 2</strong> - Opportunity Landscape plot based on Ulwick (2016) and visually inspired by Josephy (2016). All of the smartwatch micro jobs (or small tasks) are in the overserved and 'potential for disruption' part of the plot. This plot shows importance and satisfaction ratings for jobs completed on a smartwatch. 73 – 75 respondents per question. Plotted using an R script custom built by F. MacNeill. <a href="http://www.fionamacneill.co.uk/blog/2018/03/ux-camp-brighton-2018-jobs-to-be-done-r/" target="_blank" title="Blog post opens in new tab/window">Blog post from 2018</a> featuring more information. Original data is included in <a href="#table-2">Table 1</a> in the <a href="#data">Data section</a>.</p>

### Personas and low fidelity prototypes
During the second interviews, user personas based on the scenarios of a hip replacement and a cesarian section were used to consider the viability of the data and information from smartwatches. Low fidelity prototypes of mocked-up data outputs based on the actual data available from a smartwatch, were used with participants to consider *how* the data could be shown.

{{< gallery album="wfh-persona" >}}

<p class="gallery-custom-caption"><strong>Gallery Image 3</strong> - Persona for Val Lucas, a fictional patient on a care plan for a hip replacement. This persona was based on data from the National Joint Registry (NJR) who track and provide demographics related to joint replacement surgery. Created using Sketch app. <a href="val-lucas-hip-replacement.pdf" target="_blank" title="Val Lucas persona PDF opens in a new tab/window">Link to PDF for Val Lucas persona</a>.
</p>
<p class="gallery-custom-caption"><strong>Gallery Image 4</strong> - Persona for Gemma Jarrett, a fictional patient on a care plan for a caesarian section. This persona was based on NHS publications. Created using Sketch app. <a href="gemma-jarrett_csection.pdf" target="_blank" title="Gemma Jarrett persona PDF opens in a new tab/window">Link to PDF for Gemma Jarrett persona</a>.
</p>

## Outcomes
The results pointed to several key areas of opportunity, these were later validated by features and sensors added to the Apple Watch and WatchOS. The project received a mark of distinction.

### Answer to Problem Statement
**Question**: *Could information from patient-owned smartwatches and smartphones be used to support perioperative care?*

**Answer**: Yes, with patient informed consent and an appropriate means to deliver information securely to healthcare professionals a patient’s smartwatch and smartphone could be used for this purpose.

{{< gallery album="wfh-recommendations" >}}

<p class="gallery-custom-caption">
    <strong>Gallery Images 5, 6, 7</strong> - visualisation of the final recommendations as a reporting stack for software development.</p>
    <p class="gallery-custom-caption">
    <strong>Image 5 - Patient</strong>:</p> 
    <ul class="gallery-custom-list">
        <li class="gallery-custom-list-statement">IF the patient meets the criteria:</li>
        <li>[has a pre-existing condition];</li>
        <li>[is having an elective procedure with waiting time];</li>
        <li>[needs physio or occupational therapy(OT)];</li>
<li class="gallery-custom-list-statement"><em>AND</em> would benefit from:</li>
    <li>[adopting healthy behaviours];</li>
    <li>[having haptic reminders].</li>
        </ul>
        
<p class="gallery-custom-caption">
<strong> Image 6 - Frontline staff and Consultants</strong>:</p>

<ul class="gallery-custom-list">
    <li class="gallery-custom-list-statement">IF the frontline staff and Consultants need to:</li>
    <li>[encourage and monitor healthy behaviours];</li>
    <li>[provide physio or OT - in-person or remotely];</li>
    <li>[are monitoring outcomes after surgery in relation to pre-specified elective care plans].</li>
</ul>
<p class="gallery-custom-caption">
<strong>Image 7 - Warehousing and Auditing</strong>:</p>
<ul class="gallery-custom-list">
    <li class="gallery-custom-list-statement">IF senior managers and auditors need to ask the following questions of the data:</li>
    <li>[does this intervention help to prevent readmission?];</li>
    <li>[how do patients in the wearable device programme compare to those who are not? Are their outcomes better?];</li>
    <li>[what can be learned from the anonymised data?].</li>
</ul>

## Feedback
The clinical practice location where healthcare professionals had been involved in the research invited me back to present my findings. Visual design artefacts including the service design blueprint were included in a juried exhibition at the University of Brighton in 2019 (*Show and Tell - The Image in Research*). I presented as part of a UX Brighton evening event (12/02/19).

<figure class="quotation">
"...a careful combination of two different charts - a service blueprint mapping a patient's journey before, through and after surgery, matched with a mental model, which is designed to gain insight from interview transcripts...Complex information...are brought into useful arrangements for further thinking to take place. They derive from research; but they also allow research to move on from them."

<figcaption>
    &mdash; Francis Hodgson, <br/>curator of <cite>Show and Tell - The Image in Research</cite>, exhibition catalogue (2019, p.29).
</figcaption>
</figure>

## Reflection
An integral aspect of the project’s success was adopting recognised methods as a framework for the research. I used British Standards Institution’s (BSI) <cite>BS EN ISO 9241-210:2010: Ergonomics of human- system interaction. human-centred design for interactive systems</cite>. The field of user experience design research was not well known in the clinical context so the standard gave credence to the methods being used.

Had I continued this research I would have validated the Service Blueprint and mental model with a greater number of healthcare professionals working in perioperative care, specifically physiotherapists.

One of the key outstanding issues, as of writing this case study in 2021, is that Apple WatchOS does not allow the user to set rest days/dates. This  means that any health-focused app could be undermined by that aspect of the WatchOS. There are however many potential benefits for a seasoned smartwatch user who could ignore or adjust activity reminders alongside a customised app for a patient's surgical journey.

## Data

### Table 1
Smartwatch Device Ownership per Age group (data for Gallery Image 1). Smartwatch devices per Age group are listed in alphabetical order.
<table>
<caption>Column one shows the age group. Column two shows the brand of devices owned by that age group. Column three shows the count of devices, as in how many of each device brand are owned by each age group.</caption>
    <col>
    <col>
    <thread>
    <tr>
    <th scope="col">Age</th>
    <th scope="col">Device</th>
    <th scope="col">Count</th>
    </tr>
        </thread>
    <tbody>
    <tr>
      <th rowspan="3" scope="rowgroup">16-24</th>
      <th scope="row">Apple</th>
      <td>5</td>
    </tr>
    <tr>
      <th scope="row">Fitbit</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Samsung</th>
      <td>1</td>
    </tr>
  </tbody>
  <tbody>
    <tr>
      <th rowspan="6" scope="rowgroup">25-34</th>
      <th scope="row">Apple</th>
      <td>9</td>
    </tr>
    <tr>
      <th scope="row">Fitbit</th>
      <td>2</td>
    </tr>
    <tr>
      <th scope="row">Garmin</th>
      <td>2</td>
    </tr>
    <tr>
      <th scope="row">LG</th>
      <td>2</td>
    </tr>
     <tr>
      <th scope="row">Pebble</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Sony</th>
      <td>1</td>
    </tr>
  </tbody>
  <tbody>
    <tr>
      <th rowspan=9 scope="rowgroup">35-44</th>
      <th scope="row">Apple</th>
      <td>11</td>
    </tr>
    <tr>
      <th scope="row">Fitbit</th>
      <td>3</td>
    </tr>
    <tr>
      <th scope="row">Garmin</th>
      <td>3</td>
    </tr>
    <tr>
      <th scope="row">LG</th>
      <td>1</td>
    </tr>
     <tr>
      <th scope="row">Mobvoi</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Motorola</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Pebble</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Samsung</th>
      <td>4</td>
    </tr>
    <tr>
      <th scope="row">Sony</th>
      <td>1</td>
    </tr>
  </tbody>
      <tbody>
    <tr>
      <th rowspan=6 scope="rowgroup">45-54</th>
      <th scope="row">Apple</th>
      <td>13</td>
    </tr>
    <tr>
      <th scope="row">Fitbit</th>
      <td>4</td>
    </tr>
    <tr>
      <th scope="row">Garmin</th>
      <td>3</td>
    </tr>
    <tr>
      <th scope="row">Pebble</th>
      <td>1</td>
    </tr>
     <tr>
      <th scope="row">Samsung</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Sony</th>
      <td>2</td>
    </tr>
  </tbody>
  <tbody>
    <tr>
      <th rowspan=2 scope="rowgroup">55-64</th>
      <th scope="row">Apple</th>
      <td>5</td>
    </tr>
    <tr>
      <th scope="row">Garmin</th>
      <td>1</td>
    </tr>
  </tbody>
   <tbody>
    <tr>
      <th>65-74</th>
      <th>Apple</th>
      <td>2</td>
    </tr>
  </tbody>
</table>

### Table 2
Opportunity Landscape plot based on Ulwick (2016) and visually inspired by Josephy (2016) (data for Gallery Image 2). 

Jobs completed on a Smartwatch ordered from highest importance and satisfaction, to lowest.

<table>
    <caption>Column one specifies the job that can be completed on a smart watch. Columns two and three provide the Importance and Satisfaction scores. Column four, Oportunity Score is a calculation: outcome importance + (outcome importance – outcome satisfaction) = Opportunity Score</caption>
	<tr>
		<th>Micro Job</th>
		<th>Importance</th>
		<th>Satisfaction</th>
        <th>Opportunity Score</th>
	</tr>
	<tr>
		<td>Look at time</td>
		<td>9.6</td>
		<td>9.7</td>
        <td>9.5</td>
	</tr>
    <tr>
		<td>Review notifications</td>
		<td>8.4</td>
		<td>8.7</td>
        <td>8.0</td>
	</tr>
    <tr>
		<td>Log exercise</td>
		<td>7.9</td>
		<td>8.9</td>
        <td>7.0</td>
	</tr>
    <tr>
		<td>Review activity</td>
		<td>7.9</td>
		<td>9.2</td>
        <td>6.7</td>
	</tr>
    <tr>
		<td>Using apps</td>
		<td>5.3</td>
		<td>7.5</td>
        <td>3.2</td>
	</tr>
    <tr>
		<td>Check emails</td>
		<td>4.5</td>
		<td>6.3</td>
        <td>2.8</td>
	</tr>
    <tr>
		<td>Review heart rate</td>
		<td>5.3</td>
		<td>8.0</td>
        <td>2.7</td>
	</tr>
    <tr>
		<td>Check Social Media</td>
		<td>4.5</td>
		<td>6.6</td>
        <td>2.4</td>
	</tr>
    <tr>
		<td>Pay by Touch</td>
		<td>2.8</td>
		<td>4.3</td>
        <td>1.3</td>
	</tr>
    <tr>
		<td>Text messaging</td>
		<td>3.4</td>
		<td>5.9</td>
        <td>0.8</td>
	</tr>
    <tr>
		<td>Unlock by proximity</td>
		<td>2.3</td>
		<td>5.0</td>
        <td>-0.3</td>
	</tr>
     <tr>
		<td>Unlock voice control</td>
		<td>1.9</td>
		<td>4.4</td>
        <td>-0.6</td>
	</tr>
</table>

## References

<p class="referencing-style">
    British Standards Institution (BSI) (2010) <em><a href="https://shop.bsigroup.com/ProductDetail/?pid=000000000030186637" target="_blank" title="BSI opens in new tab/window">BS EN ISO 9241-210:2010: Ergonomics of human- system interaction. human-centred design for interactive systems</a></em>. (Accessed: 2 September 2018).
</p>

<p class="referencing-style">
    Josephy, J. (2016) ‘Jobs to be done – a better way to innovate’, <em><a href="https://www.webcredible.com/blog/may16-jobs-be-done-better-way-innovate/" target="_blank" title="Webcredible blog opens in new tab/window">Webcredible blog</a></em>. Available at:  (Accessed: 23 March 2018).
</p>

<p class="referencing-style">
    Royal College of Anaesthetists (RCoA) (2014) <em>Perioperative medicine the pathway to better surgical care</em>.(Accessed: 31 July 2018).
</p>

<p class="referencing-style">
    Stickdorn M. et al. (2018) <em>This is service design doing</em>. 1st edn. Sebastopol, CA, USA: O’Reilly Media.
</p>

<p class="referencing-style">
    Ulwick, A.W. (2016) <em><a href="http://amzn.eu/7BpXFp0" target="_blank" title="Amazon opens in new tab/window">Jobs to be Done: Theory to practice</a></em>. (Downloaded: 3 March 2017).
</p>

<p class="referencing-style">
    Viera, K. and Tomlinson, T. (2019) Blackboard keynote [PowerPoint]. <em>19th Durham Blackboard Users’ Conference</em>. Unpublished presentation.
</p>

<p class="referencing-style">
    Wickham, H. (2016). <em>ggplot2: Elegant graphics for data analysis</em>. 2nd edn. New York, USA: Springer.
</p>

<p class="referencing-style">
    Young, I. (2008) <em>Mental models: Aligning design strategy with human behavior</em>. New York, USA: Rosenfeld Media.
</p>


