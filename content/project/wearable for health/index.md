---
title: Wearable for Health
summary: Smartwatches and smartphones to support surgery

tags:
- Research
date: "2021-07-16T00:00:00Z"
type: "book"

gallery_item:
- album: survey
  image: devicebyage.png
  caption: Image 1 - Smartwatch brand distribution by age group as a bar chart. 
  alt_text: does this work
- album: survey
  image: opplandhealth.png
  caption: Image 2 - Opportunity Landscape plot featuring diagonal lines to show sectors of opportunity.

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
This user research project explored the use of information from patient-owned smartwatches and smartphones to support patient care prior to surgery. The project also assessed the informational needs of healthcare professionals, asking what data sources they would need from patients' smartwatches and smartphones to support care. Through the project research, I identified improvements which were later added to Apple WatchOS and Apple Health for iPhone. These included separating walking and running data, automatically detecting workouts, and providing relational data such as walking distance per day.

The completed [Service Blueprint can be viewed at LucidChart.](https://lucid.app/documents/view/7a5f0dd2-3e17-45cc-b81c-4dee3d6b8cc9) Link opens in a new tab/window. 

![Iterative development of the Service Blueprint diagram presented in a chronological list](blueprint_iterations.png "Overview of the iterative development of the Service Blueprint used with participants as a means to understand and discuss a patient's journey. The printed version of the Service Blueprint is over two metres wide and is designed to be viewed as a long poster. It was created using LucidChart.")

## Background
While completing an MSc in 2018 I used my dissertation project as an opportunity to explore a real-world area of user research; wearable devices in digital health. The project focused on healthcare professionals as a user group initially to ascertain if the information from these devices was fit for purpose prior to creation of apps and software. The research was ethically approved and took place in a clinical location. The research took place over a 6-month period.
![System map for Apple Health, with devices and infrastructure. Caption includes description.](applehealthapp-system.jpg "The Apple Health app ecosystem is reliant on infrastructure provided by a healthcare provider. Inspired by ‘system maps’ in Stickdorn *et al.* (2018), This is Service Design Doing, pp. 58-63. Created using Adobe Illustrator CC as part of a competitor analysis. </br></br> Dotted lines indicate two-way data exchange and read/write relationship.</br> P ~ Patient, and HCP ~ Healthcare Professional.")


## Objective
To use the problem statement as the basis for an in-depth speculative user experience study to be written up as a dissertation and disseminated back to the UX and healthcare communities.

### Problem Statement
*Could information from patient-owned smartwatches and smartphones be used to support perioperative[^1] care?* 

[^1]: *Perioperative* ~ Encompasses the period prior to surgery, during surgery and through to the conclusion of recovery at home; as defined by the Royal College of Anaesthetists (RCoA, 2014, pp. 4-5).

## Roles, Methods, and Tools
I was main researcher on this project. My work was overseen by two supervisors: one supervisor was from a UX/academic background (named principal investigator), and one from a medical practice background, whom I actively sought out to support the project.

### Highlighted methods
<ul>
    <li><a href="#interviews">Interviews</a></li>
    <li><a href="#survey-of-smartwatch-owners">Survey and Quantitative Analysis</a></li>
    <li><a href="#personae-and-low-fidelity-prototypes">Personae</a></li>
</ul>

#### Interviews
In preparation for field work, I engaged in interviews with professional contacts whom had relevant healthcare experience. I co-created a Service Blueprint diagram outlining the patient journey. I also created a glossary, based on the qualitative data from interviews, to ensure that descriptive terms used in the recruitment materials, oral presentations and dissertation were contextually accurate and appropriate.

Alongside this I formed a research collaboration with a healthcare professional working in a relevant role in practice. My collaborator helped to facilitate contextual interviews with healthcare professionals working in a clinical setting. These interviews were used as the basis for discovering data/information requirements. Second interviews were completed with the same participants. A lightweight card sorting exercise was used in the first interview to determine which types of health information were pertinent and in order of importance.

![Interview kit on a table, with do not disturb sign, pens, post-its, and a card sorting exercise'](research-wearable-for-health.jpg "Lightweight interview kit. Designed to be taken to a room in a clinical practice location and quickly picked up if needsbe. Cards were based on the core information types available from a smartwatch/smartphone, e.g., heart rate, exercise time, step count, etc. Cards created using Adobe Illustrator CC.")

#### Survey of Smartwatch owners
I designed a survey, to gauge the attitudes of current smartwatch owners in relation to use of devices for health related purposes. The survey was distributed via online user communities, social media, and via targeted emails. The quantitative findings were presented in the dissertation and used to inform the list and prioritisation of requirements. The open-text responses were used as part of human-factors, looking at the likelihood of technology adoption and potential risks.

{{< gallery album="survey" >}}


**Gallery Image 1** - 75 survey respondents. A key observation is that the 45-54 age group holds the second highest proportion of ownership. These users will be entering the age-based demographics for procedures such as joint replacement over the next 12-20 years. Plotted using RStudio and ggplot2 (Wickham, 2016). Original data is included in [Table 1](#table-1) in the [Data](#data) section
</br></br>
**Gallery Image 2** - Opportunity Landscape plot based on Ulwick (2016) and visually inspired by Josephy (2016). All of the smartwatch micro jobs (or small tasks) are in the overserved and 'potential for disruption' part of the plot. This plot shows importance and satisfaction ratings for jobs completed on a smartwatch. 73 – 75 respondents per question. Plotted using an R script custom built by F. MacNeill. [Blog post from 2018](http://www.fionamacneill.co.uk/blog/2018/03/ux-camp-brighton-2018-jobs-to-be-done-r/) featuring more information. Original data is included in [Table 2](#table-2) in the [Data](#data) section.
{style="font-size: 16px"}


#### Personae and low fidelity prototypes
During the second interviews user personas with the scenarios of a hip replacement and a cesarian section were used to consider the viability of the data and information from smartwatches. Low fidelity prototypes of mocked-up data outputs based on the actual data available from a smartwatch, were used with participants to consider *how* the data could be shown.

[Example personae - include software that was used]

### Outcomes

The results pointed to several key areas of opportunity, these were later validated by features and sensors added to the Apple Watch and WatchOS. The project received a mark of distinction.

### Answer to Problem Statement
**Question**: *Could information from patient-owned smartwatches and smartphones be used to support perioperative care?*

**Answer**: Yes, with patient informed consent and an appropriate means to deliver information securely to healthcare professionals a patient’s smartwatch and smartphone could be used for this purpose.

[Visual summary of the final recommendations Include edited version of the stack slide]

## Feedback

The clinical practice location where healthcare professionals had been involved in the research invited me back to present my findings. Visual design artefacts including the service design blueprint were included in a juried exhibition at the University of Brighton in 2019 (*Show and Tell - The Image in Research*). I presented as part of a UX Brighton evening event (12/02/19).

>"...a careful combination of two different charts - a service blueprint mapping a patient's journey before, through and after surgery, matched with a mental model, which is designed to gain insight from interview transcripts...Complex information...are brought into useful arrangements for further thinking to take place. They derive from research; but they also allow research to move on from them."

Francis Hodgson, curator 
Excerpt from *Show and Tell - The Image in Research*, exhibition catalogue (2019, p.29).

[Include image of mental model and link though to that]

## Reflection
An integral aspect of the project’s success was adopting recognised methods as a framework from the research. I used British Standards Institution’s (BSI) *BS EN ISO 9241-210:2010: Ergonomics of human- system interaction. human-centred design for interactive systems*. The field of user experience design research was not well understood in a clinical context so this helped to validate the methods being used, providing an overview.

Had I continued this research I would have liked validated the Service Blueprint and mental model with a greater number of healthcare professionals working in perioperative care, specifically physiotherapists.

One of the key outstanding issues, as of writing this case study in 2021, is that Apple WatchOS does not allow the user to set rest days/dates. This  means that any health-focused app could be undermined by that aspect of the WatchOS. There are however many potential benefits for a seasoned smartwatch user who could ignore or adjust activity reminders alongside a customised app for a surgical journey.

## Data

### Table 1
Smartwatch Device Ownership per Age group (data for Gallery Image 1). Smartwatch devices per Age group are listed in alphabetical order.
<table>
<caption>Smartwatch device ownership per age group</caption>
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