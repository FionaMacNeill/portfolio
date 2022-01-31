---
title: "[Talk] Factors of Trust in IoT App Interfaces Redux"
date: "2016-06-14"
categories: 
  - "digital-literacies"
  - "iot"
  - "mobile"
  - "ui"
  - "ux"
tags: 
  - "accessibility"
  - "android"
  - "apps"
  - "dashboard"
  - "interaction"
  - "ios"
  - "mobile"
  - "mobile-devices"
  - "mobile-technology"
  - "msc"
  - "scenarios"
  - "ux"
  - "wearables"
coverImage: "Screen-Shot-2016-03-19-at-09.07.10-2a9vvs5.png"
---

## Talk presented at UX Camp Brighton 2016 - Redux on 14/06/16 at 68 Middle Street

[http://uxbrighton.org.uk/](http://uxbrighton.org.uk/) [See original blog post](http://fionamacneill.co.uk/blog/2016/03/19/talk-factors-of-trust-in-iot-app-interfaces/) for the version of this talk given at UX Camp Brighton, 2016 (19/03/16). Video version of original talk.[FACTORS OF TRUST IN IOT APP INTERFACES](https://vimeo.com/160628235) from [Fiona MacNeill](https://vimeo.com/user10479357) on [Vimeo](https://vimeo.com). 

<iframe src="https://player.vimeo.com/video/160628235" width="800" height="600" frameborder="0" allowfullscreen="allowfullscreen"></iframe>

## Session description:

Does your app rely on OAuth to offer connection to other apps and services? Based on my research studying app-to-device relationships in Internet of Things systems (e.g. Fitbit, Jawbone UP, Nest, SmartThings, Glooko), I have uncovered some best practice recommendations when it comes to inspiring trust within your interface. Trust definitions used in this video are from Pavlidis, Islam, Mouratidis, and Kearney (2014). This research is aligned with the SenSe research Cluster at the University of Brighton (secure and dependable software systems). 

## About SenSe

[The SenSe cluster](https://www.brighton.ac.uk/research/our-research/life-health-and-physical-sciences/research-groups/computing/index.aspx) aims to develop novel and pragmatic ways to assure the dependability of software systems with particular emphasis on security, trust and risk. We focus on theories from model-based engineering and analysis-based assurance to develop methods, models, practices and tools that promote the provision of security and dependability in complex interconnected and heterogeneous systems and information infrastructures that underpin our economy and society. 

## Preliminary recommendations:

UX Questions to Ask in Relation to IoT Apps

<table><tbody><tr><td>#</td><td>Category</td><td>Questions to ask</td></tr><tr><td>1</td><td><strong>System dialogues and Semantics</strong></td><td>Are system dialogues consistent?<ul><li>For data permissions</li><li>for use tips</li><li>for motivational messages</li></ul></td></tr><tr><td>2</td><td><strong>Settings</strong></td><td>Are all the settings housed together? Are items like the privacy policy and standards adherence available from this area? Can the Terms of Service (or a shortened format of ToSs) be accessed from within the app? Can connected apps and devices be reviewed/managed from within the app? Can support documentation be accessed from within the app?</td></tr><tr><td>3</td><td><strong>Checkups for Setup/Workflow/Privacy </strong>An essential part of onboarding. Also a method for supporting trust and helping users to invest time in learning the higher-level functions of an app, which promotes realisation of app benefits and long-term commitment to use of the app (Brignull, 2013).<strong></strong></td><td><strong>Periodic reminders about setup:</strong><ul><li>Can the setup be improved?</li><li>What devices could be added safely?</li><li>What benefits might be available as part of the system that the user may be unaware of?</li></ul><strong>Periodic review of workflow: </strong>ask users to review the workflow in the system to add a level of human oversight. If the app is not accessed frequently then email and text message may be effective ways to prompt engagement. Think of it like entering a monthly gas meter reading.<strong></strong><ul><li>Is an automated workflow still operating as intended?</li><li>Is the function still needed?</li></ul>A possible incentive could be that the workflow will stop/timeout if it is not reviewed a la IFTTT.<strong> </strong><strong>Periodic review of p</strong><strong>rivacy: </strong>privacy overview and audit tools within the app.<ul><li>What information is shared with third-party developers?</li><li>For what purpose/s is it shared?</li></ul>Non-legalese overview of changes to T&Cs should be included in privacy checks.</td></tr><tr><td>4</td><td><strong>Role/function of the app </strong>Applies to central app and third-party apps.</td><td>This sounds really obvious, but a lot of primary IoT apps don't actually explain their purpose within the system. What service does the app offer? What need does the app fulfill? What does the app do? How important is the app to the operation of the system? E.g. is it the primary interface or management tool for the system? What data does it need? - Make it clear what is used and why, in plain English.</td></tr><tr><td>5</td><td><strong>Health/status of hub/sensor/device </strong>At any point in time the user should be able to view a basic log of what is currently going on in the system.<strong></strong></td><td>What is going on in the system right now? Is recent system activity accessible? Is it possible to access logs from other time periods? Is it possible to see what communication channels are in operation? What third-party apps are connected to the system, what are they doing? What third-party devices are connected to the system, what are they doing? This should be more like what you expect from your banking app when it comes to overseeing the operation of high-importance health, home/business automation IoT systems.</td></tr><tr><td>6</td><td><strong>OAUTH and API: secondary app data use</strong></td><td>Respect users and prove that your app is more trustworthy by only calling data that you are actually using. What data is needed into order to provide the desired third-party service? How is the data used to provide the service? <strong>Note:</strong> platform manufacturers/developers need to ensure that third-party apps aren't over-privileged in terms of the data they access and the calls they can make via APIs (See the work of  Fernandes, Jung and Prakesh, 2016). Developers need to state their intention when it comes to use of information that they call via the API. This doesn't stop those with malicious intent, but it helps users to distinguish between those who pay due diligence to privacy and those who are either malicious or sloppy.</td></tr><tr><td>7</td><td> <strong>What is shared?</strong></td><td>Can data access be allowed/disallowed? Once disallowed from the primary app, is this decision upheld? <strong>Ideal world:</strong> provide granular options for allowing/disallowing access to data which is not necessary for the operation of the service offered by the app. Better yet, don't ask for the data at all if it isn't essential to operation.</td></tr><tr><td>8</td><td><strong>Access control</strong></td><td>Is two-step authentication an option for the web app and login from a new device? Does the smartphone/tablet app offer biometric authentication? Does the app offer the option of setting a passcode for auto screen lock? Particularly if the app controls home appliances.</td></tr><tr><td>9</td><td><strong>Dependency and operational relationship</strong></td><td>As systems become more complicated it is crucial that the user is aided in building a mental picture of the basic configuration of the system. I [keep thinking of Max](https://cycling74.com/products/max/) when I think of this issue. Is logging available? What is going on in the system right now? What is attached to this system (devices/sensors/users)? Is the system visualised in any way?</td></tr><tr><td>10</td><td><strong>Try before you buy</strong></td><td>Wearables have the right idea on this one, allowing you to trial a wearable companion app using your smartphone's built-in sensors. What if you could try out the perks of the system before you buy the actual device? Is a preview of how the app will operate with devices, provided as part of onboarding? Can you try of some of the functionality of the system without buying a system-specific device?</td></tr></tbody></table>

## References

\[alex\]. (2016, May 2). _SmartThings platform security - response from Alex_. Retrieved June 13, 2016, from [https://community.smartthings.com/t/smartthings-platform-security-response-from-alex/46878](https://community.smartthings.com/t/smartthings-platform-security-response-from-alex/46878) 

Aliph, Inc. (2016). Jawbone UP (Version 4.13) \[Mobile application software\]. Retrieved from [https://itunes.apple.com/gb/app/up-by-jawbone-track-up-move/id461125277?mt=8](https://itunes.apple.com/gb/app/up-by-jawbone-track-up-move/id461125277?mt=8) 

Barcena, M. B., Wueest, C., & Lau, H. (2014). How safe is your quantified self? (1.1). Retrieved from [http://www.symantec.com/content/en/us/enterprise/media/security\_response/whitepapers/how-safe-is-your-quanti fied-self.pdf](http://www.symantec.com/content/en/us/enterprise/media/security_response/whitepapers/how-safe-is-your-quantified-self.pdf) 

BBC (2016). _Hidden killers, series 1: 2. The Edwardian home_ Retrieved from [http://www.bbc.co.uk/iplayer/episode/b03lyv9x/hidden-killers-series-1-2-the-edwardian-home](http://www.bbc.co.uk/iplayer/episode/b03lyv9x/hidden-killers-series-1-2-the-edwardian-home) 

Bilton, N. (2016, January 18). Nest thermostat glitch leaves users in the cold. The New York Times. Retrieved from [http://www.nytimes.com/2016/01/14/fashion/nest-thermostat-glitch-battery-dies-software-freeze.html](http://www.nytimes.com/2016/01/14/fashion/nest-thermostat-glitch-battery-dies-software-freeze.html) 

Bradbury, D. (2015, November 26). Usability v safety: How to design our way to better security. The Guardian. Retrieved from [https://www.theguardian.com/media-network/2015/nov/26/usability-safety-how-to-design-better-security-technology](https://www.theguardian.com/media-network/2015/nov/26/usability-safety-how-to-design-better-security-technology) 

Brooks, J. (2016, January 8). Fitbit hit with class action lawsuit over alleged misreading of heart rates \[Blog post\]. Retrieved from [http://ww2.kqed.org/futureofyou/2016/01/08/fitbit-hit-with-class-action-lawsuit-over-alleged-misreading-of-heart-rates/](http://ww2.kqed.org/futureofyou/2016/01/08/fitbit-hit-with-class-action-lawsuit-over-alleged-misreading-of-heart-rates/) 

Brignull, H. (2013, March). _Ramp Up_. Personalising the experience, Brighton. Retrieved from [http://uxbrighton.org.uk/Personalisation-the-Experience/](http://uxbrighton.org.uk/Personalisation-the-Experience/) 

Brignull, H. (2016). _User interfaces designed to trick people_. Retrieved June 13, 2016, from [http://darkpatterns.org/](http://darkpatterns.org/)

BS ISO/IEC. (2011). Systems and software engineering — Systems and software quality requirement and evaluation (SQuaRE) — System and software quality models (ISO/IEC 25010:2011(E)) Switzerland: ISO/IEC 

Catalyst IT. (2016). Mahara (Version 1.10.5) \[Computer software\]. Retrieved from [http://mahara.org](http://mahara.org) 

Chen, E. Y., Pei, Y., Chen, S., Tian, Y., Kotcher, R., & Tague, P. (2014). OAuth Demystified for mobile application developers. _CCS ’14 Proceedings of the 2014 ACM SIGSAC Conference on Computer and Communications Security_. doi:[10.1145/2660267.2660323](http://dl.acm.org/citation.cfm?doid=2660267.2660323) 

Cluley, G. (2013, February 13). Jawbone accounts compromised by hackers - personal info accessed, passwords disabled \[Blog post\]. Retrieved from [https://nakedsecurity.sophos.com/2013/02/13/jawbone-hack/](https://nakedsecurity.sophos.com/2013/02/13/jawbone-hack/) 

Cycling’74. _Max is a visual programming language for media_. Retrieved March 19, 2016, from [https://cycling74.com/products/max/](https://cycling74.com/products/max/) 

Ericsson. (2016, June). _Wearable technology and the Internet of things_. Retrieved from [https://www.ericsson.com/thinkingahead/consumerlab/consumer-insights/wearable-technology-and-the-internet-of-things](https://www.ericsson.com/thinkingahead/consumerlab/consumer-insights/wearable-technology-and-the-internet-of-things) 

Faily, S. (2014). Engaging stakeholders in security design: An assumption-driven approach. Proceedings of the Eighth International Symposium on Human Aspects of Information Security & Assurance (HAISA 2014), Plymouth, 21-29. doi:10.13140/2.1.3997.2647 

Feamster, N. (2016, January 19). Who will secure the Internet of things? \[Blog post\]. Retrieved from [https://freedom-to-tinker.com/blog/feamster/who-will-secure-the-internet-of-things/](https://freedom-to-tinker.com/blog/feamster/who-will-secure-the-internet-of-things/) 

Felt, A. P., Egelman, S., & Wagner, D. (2012). I’ve got 99 problems, but vibration ain’t one. _Proceedings of the second ACM workshop on Security and privacy in smartphones and mobile devices - SPSM ’12_. doi:[10.1145/2381934.2381943](http://dl.acm.org/citation.cfm?doid=2381934.2381943) 

Field, C. (2004, January 23). Danger high voltage! Edwardian electric Tablecloth uncovered Retrieved from [http://www.culture24.org.uk/history-and-heritage/art19432](http://www.culture24.org.uk/history-and-heritage/art19432) 

Fitbit, inc. (2016). Fitbit (Version 2.18) \[Mobile application software\]. Retrieved from [https://itunes.apple.com/gb/app/fitbit/id462638897?mt=8](https://itunes.apple.com/gb/app/fitbit/id462638897?mt=8) 

Guadamuz, A. (2015). The monkey selfie: Copyright lessons for originality in photographs and internet jurisdiction. _Internet Policy Review_. doi:[10.14763/2016.1.398](http://policyreview.info/articles/analysis/monkey-selfie-copyright-lessons-originality-photographs-and-internet-jurisdiction) 

Glooko, Inc. (2015). Glooko (Version 3.2) \[Mobile application software\]. Retrieved from [https://itunes.apple.com/gb/app/glooko/id471942748?mt=8](https://itunes.apple.com/gb/app/glooko/id471942748?mt=8) 

Harrison, D., Marshall, P., Bianchi-Berthouze, N., & Bird, J. (2015). Activity tracking: Barriets, workarounds and customisation. Proceedings of UBICOMP ‘15, Osaka, Japan. doi:10.1145/2750858.2805832 

Hess, W. (2015, May 7). _Onboarding: Designing Welcoming First Experiences_. Retrieved March 19, 2016, from [http://uxmag.com/articles/onboarding-designing-welcoming-first-experiences](http://uxmag.com/articles/onboarding-designing-welcoming-first-experiences) 

Higginbotham, S. (2016, January 22). Episode 42: These are the two biggest challenges facing the smart home Retrieved from [http://iotpodcast.com/2016/01/episode-42-these-are-the-two-biggest-challenges-facing-the-smart-home/](http://iotpodcast.com/2016/01/episode-42-these-are-the-two-biggest-challenges-facing-the-smart-home/) 

Higginbotham, S. (2016, March 17). _Episode 50: Are your devices being held hostage?_. Retrieved March 28, 2016, from [http://iotpodcast.com/2016/03/nest-hostage/](http://iotpodcast.com/2016/03/nest-hostage/) 

Internet Policy Review. (2013). _Privacy & security_. Retrieved June 13, 2016, from [http://policyreview.info/categories/privacy-security](http://policyreview.info/categories/privacy-security) 

IoT security research at university of Michigan. (2016). Retrieved June 13, 2016, from [https://iotsecurity.eecs.umich.edu/](https://iotsecurity.eecs.umich.edu/) 

Kastrenakes, J. (2016, March 10). Nest can now use your phone to tell when you’ve left the house Retrieved from [http://www.theverge.com/2016/3/10/11188888/nest-now-uses-location-for-home-away-states-launches-family-accounts](http://www.theverge.com/2016/3/10/11188888/nest-now-uses-location-for-home-away-states-launches-family-accounts) 

Kalloniatis, C., Mouratidis, H., Vassilis, M., Islam, S., Gritzalis, S., & Kavakli, E. (2014). Towards the design of secure and privacy-oriented Information Systems in the Cloud: Identifying the major concepts. Computer Stan- dards & Interfaces, 36(4), 759–775. doi:10.1016/j.csi.2013.12.010 

Krok, A. (2016, June 6). _British security firm hacks Mitsubishi Outlander via mobile app, Wi-Fi - Roadshow_. Retrieved June 12, 2016, from [http://www.cnet.com/roadshow/news/british-security-firm-hacks-mitsubishi-outlander-via-mobile-app-wi-fi/](http://www.cnet.com/roadshow/news/british-security-firm-hacks-mitsubishi-outlander-via-mobile-app-wi-fi/) 

Lohr, S. (2016, June 9). Tony Fadell steps down amid tumult at nest, a Google acquisition. _Technology_. Retrieved from [http://www.nytimes.com/2016/06/04/technology/tony-fadell-nest-google-alphabet.html](http://www.nytimes.com/2016/06/04/technology/tony-fadell-nest-google-alphabet.html) 

Malik, O. (2015, December 30). In Silicon valley now, it’s almost always winner takes all. _The New Yorker_. Retrieved from [http://www.newyorker.com/tech/elements/in-silicon-valley-now-its-almost-always-winner-takes-all](http://www.newyorker.com/tech/elements/in-silicon-valley-now-its-almost-always-winner-takes-all) 

myDevices. (2016). _First IoT project builder - myDevices cayenne_. Retrieved March 19, 2016, from [https://www.cayenne-mydevices.com/](https://www.cayenne-mydevices.com/) 

Nest Labs, Inc. (2016). Nest app (Version 5.2.2) \[Mobile application software\]. Retrieved from [https://itunes.apple.com/gb/app/nest-app/id464988855?mt=8](https://itunes.apple.com/gb/app/nest-app/id464988855?mt=8) 

O’Neill, O. (2002). A question of trust: The BBC Reith lectures 2002 (4th ed.). United Kingdom: Cambridge University Press. 

O’Neill, O. (2013, September 25). How to trust intelligently \[Blog post\]. Retrieved from [http://blog.ted.com/ how-to-trust-intelligently/](http://blog.ted.com/ how-to-trust-intelligently/)

Pavlidis, M., Islam, S., Mouratidis, H., & Kearney, P. (2014). Modeling trust relationships for developing trust- worthy Information systems. International Journal of Information System Modelling and Design, 5(1), 25–48. doi:10.4018/2014010102 

openHAB. (2016). _OpenHAB_. Retrieved June 13, 2016, from http://www.openhab.org/ Rogers, C. Martha Lane Fox interviewed by the house magazine Retrieved from [https://doteveryone.org.uk/blog/2016/05/martha-lane-fox-in-the-house-magazine/](https://doteveryone.org.uk/blog/2016/05/martha-lane-fox-in-the-house-magazine/) 

Sasse, A. (2015). Scaring and bullying people into security won’t work. IEEE Security & Privacy 13(3), 80-83. doi:10.1109/MSP.2015.65 

Scoseria, I. (2016). MyDevices launches cayenne, the world’s First drag-and-drop IoT project builder. Retrieved 19 March 2016, from [http://press.mydevices.com/2016/01/26/mydevices-launches-cayenne-the-worlds-first-drag-and-drop-iot-project-builder/](http://press.mydevices.com/2016/01/26/mydevices-launches-cayenne-the-worlds-first-drag-and-drop-iot-project-builder/) 

Secure Tropos. (2013). SecTro2 (Version 2.1) \[Computer software\]. Retrieved from [http://www.omilab.org/web/secure-tropos/environment](http://www.omilab.org/web/secure-tropos/environment) 

Sempers, P. (2015, October 19). _Samsung Smartthings app tour on galaxy s6 - #ThinkSmartThings_ Retrieved from [https://www.youtube.com/watch?v=UmqmpJg\_xFA](https://www.youtube.com/watch?v=UmqmpJg_xFA) 

Seuss (1999). _The cat in the hat_ (5th ed.). New York: Random House USA Children’s Books. 

Spary, S. (2016, January 6). Online criminals are tageting Fitbit user accounts. BuzzFeed News. Retrieved from [http://www.buzzfeed.com/saraspary/online-criminals-are-targeting-fitbit-user-accounts](http://www.buzzfeed.com/saraspary/online-criminals-are-targeting-fitbit-user-accounts) 

SmartThings, Inc. (2016). SmartThings Mobile (Version 2.0.7) \[Mobile application software\]. Retrieved from [https://itunes.apple.com/gb/app/smartthings-mobile/id590800740?mt=8](https://itunes.apple.com/gb/app/smartthings-mobile/id590800740?mt=8)

Wollerton, M. (2016, May 23). The best smart hub. Retrieved from [http://thewirecutter.com/reviews/best-smart-hub/](http://thewirecutter.com/reviews/best-smart-hub/) 

Woods, B. (2016, January 19). _Hippocratic oath for connected medical devices_. Retrieved June 12, 2016, from [https://www.iamthecavalry.org/domains/medical/oath/](https://www.iamthecavalry.org/domains/medical/oath/)

## My current personal hero:

<iframe src="https://www.youtube.com/embed/Hxdqp3N_ymU" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen"></iframe>
