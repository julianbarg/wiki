[[_TOC_]]

Back to [[Oil spills]].

## Incident image

[[https://www.bellinghamherald.com/latest-news/ju0o3y/picture21815628/alternates/LANDSCAPE_1140/Pipeline_smoke.source.prod_affiliate.39.jpg|frame, alt=Incident as seen from the neighborhood, size=600px]] 
  
## Actors 
* [[Olympic Pipe Line]]
* Bayfield facility: Facility with five product tanks, presumably for storage and delivery of petroleum products.
* [[OPS]]

## Technology
* [[SCADA]]
* [[RTU]]
* [[PLC]]
* [[IMCO]]

## Summary

The pipeline was damaged in 1994 when piping was installed for a nearby water plant in 1994. Originally, Olympic Pipeline employees were supposed to be present for every part of the work. But when some employees made changes to some plans, Olympic Pipeline was not informed. The crew carried out that work by themselves, adjusting their plans as they went along. The pipeline was struck by a backhoe but did not burst [@NTSB2002 p. 24]. The Olympic Pipeline employees were on site during some of that time, but most likely failed to notice the additional excavation around the pipeline. They were also not informed of this work [@NTSB2002 p. 58]. Two analyses with smart pigs (magnetic flux and caliper tool) were carried out between the time of the damage and the eventual spill [@NTSB2002 p. 57]. These analyses picked up the damage, but Olypmic Pipeline failed to follow up and inspect the pipeline, and the supervising agencies failed to follow up and enforce action. An improperly installed relief valve did not function properly [@NTSB2002 p. 45].

At the day of the incident, a system administrator entered a faulty data entry into the server that controls the SCADA system. "The system administrator said he noticed that the records [later] contained a typographical error that he said was not there when he created them" [@NTSB2002 p. 11].  This SCADA system is used to remotely control the pipeline. It just so happened that at around the same time, the controller ran a few operations (which were routine operations) on the pipeline via the SCADA system that caused the pressure to spike [@NTSB2002 p. 3]. The pressure spiked to 1,494 psig,; it had previously been tested at 1,820psig [@NTSB2002 p. 14]. Because the SCADA system experienced problems at around the same time for about 20-30 minutes [@NTSB2002 p. 62], the operator was not able to swiftly respond to an increasing pressure [@NTSB2002 p. 62] and did not notice a sudden drop in pressure at 3:28PM--the burst of the damaged section of the pipeline [@NTSB2002 p. 5]. Later the operator attempt to resume operations, which within an additional 13 minutes of operations [@NTSB2002 p. 66] added another 1,890 barrels bein spilled, leading to a total spill of 5,638 barrels spilled [@NTSB2002 p. 11].

## Significance

Maybe around this time we see the rise of leak detection software. Interestingly, the leak detection software throws an alarm, but the controller seems to ignore it, and starts another pump. Maybe the software still needs to gain legitimacy/authority? Maybe controllers aren't very cautious, or have seen too many false positives/are conditioned to ignore the alarm? Even more interesting is that the pump is later stopped only after another employee smells gasoline odors - a truly unusual occurance [@NTSB p. 7]?

This case also introduces some of the issues we might encounter with research in this area. Those involved might fabricate technology problem narratives to cover up human errors or other sources of errors. We would keep updating the technology, while not actually adressing the underlying issue. Also, does the new, more capable technology such as the Bayfield station and SCADA systems cause us to run technology closer to its limits, such as exemplified by the high peak pressure? And what about all the technology. In theory, all this great stuff is now available, but do organizations actually upgrade? Banks run on 50 year old COBOL code, what about pipelines? Maybe, they are still using the same SCADA systems today that were used in '98, and their condition only got worse?

## Learning

### Mechanisms

### Outcomes

## The spill

## Cause analysis

### What could have been done
 
#### To prevent the spill
* Installation of proper inlet pressure relief valve [@NTSB2002 p. 68].
       
#### To reduce the severity of the spill

### Faulty parts/flawed procedures
* DOT regulations did not specify testing methods for safety equipment [@NTSB2002 p. 52].

## Aftermath/learning

### Olympic 
* Updated its manuals with regard to the Bayfield facility [@NTSB2002 p. 40].
* Various corrective action [Appendix B @NTSB2002 p. 76f].

### Regulations
* OPS rule about repairing specific damages within 60 days.

### Other
* NTSB suggesting that software changes or data input not be made on live systems [@NTSB2002 p. 64].
* NTSB suggesting users don't share logins on computers and don't all receive admin privileges [@NTSB2002 p. 62].

## My reactions
* Another incident that the PHMSA did not update on in its database. I can see why the [[commentator|Houston '94##regarding-phmsa-research-and-actiobn]] on [[Houston '94]] as well as the NTSB in general got fed up with the DOT. Assumin that the PHMSA researchers rely on the PHMSA database, it would be fair  assume that they would have a bias toward drawing on data of spills where the cause of the incident is immediately clear and reported in the PHMSA incident report. Fortunately, PHMSA changed their policy starting in 2002 and began to update the database later.
* We continue to see a response that is more focused on discussing the response. Is the message: despite the spill, the deaths should have been avoidable? So is the blame for the injuries put on the rescue personnel instead of the operator? Should rescue personnel be obliged to respon perfectly to an incidents? Is that part of our social contract?
* Procurement issues on p 36f. It seems so many things that should be routine are actually not?
* Were the controllers incompetent or malicious? They were under criminal investigation, otherwise we might have some statements from them. But this just goes to exemplify that you cannot trust the statements of those involved in general. They might fear repercussions. The bigger question is whether controllers are incompetent in general, or whether this is some case of sampling bias. What if the technology piece is just a coverup?
* It seems the starting point for OPS (as for any inspector it seems) is the status quo of the organization. Are the regulations just a reference point that practice converges toward, but that it never reaches? Whenever a failure occurs, action may be taken to correct the underlying issues, but at the same time, performance could get worse in other areas.
* On the one hand, for an incident to occur, it really requires a combination of multiple unlikely events. On the other hand, the reports show negligence of misconduct in every organizational function involved, so how unlikely is the occurance of unlikely events really?
* There is a pattern of too many alarms and false positive.

## Various
   
*A story as old as time:  
 
> The system administrator said he noticed that the records now contained a typographical error that he said was not there when he created them. [@NTSB2002 p. 7]

* Most of the IMCO employees did not spill the beans on their colleagues [@NTSB2002 p. 25].

> Because the SCADA screens for Bayview were still under development 6 months after the facility’s startup, no pressure trend SCADA screen for Bayview was readily available to the accident controller.

* I could easily believe that the the feature is still under development 10 years later.
* If regulations not followed up on, who is really to be blamed? The regulator steered himself clear of guilt, but regulations without enforcement are really meaningles. ALso, what role does wanting to keep the industry profitable play in these issues.

> Indeed, any improvements in pipeline operations between the Bayview commissioning and the accident were apparently the 
result of trial-and-error experiences of the controllers, not the result of effective management oversight. [@NTSB2002 pp. 68f]

## Documents

### NTSB report

* [[http://www.ntsb.gov/investigations/AccidentReports/Reports/PAR0202.pdf]]

### News reports    
* [[https://www.kiro7.com/news/north-sound-news/on-this-day-olympic-pipeline-explosion-in-bellingham-kills-three-in-1999/766933436/]]
 
### Relevant laws and regulations

### Videos

### Other

## Data

### PHMSA narrative

> "Mainline 16\" pipline rupture.  Cause is being investigated by the ntsb and dot office of pipeline safety.  Initial examination of the pipe revealed a 28\" longintudinal spill and gouges and dents adjacent to the rupture area.  Details to be provided following the ntsb investigation.  Supplemental info:  mainline 16\" pipeline ruptured.  Initial examination of the failed pipe revealed at 28\" longitudinal split with gouges and dents adjacent to the rupture area.  The impact of this damage on the pipes failure, as well as all other potential causes including the functioning of surge relief equipment, is under current investigation by the ntsb and the dot office of pipeline safety."

### Quantitative data

According to the PHMSA dataset, the line had been tested for a pressure of 1,620 psig.

|**General information**
|----------------|---:
|Incident ID:    |19990107
|Operator name:  |Olympic Pipe Line Company
|Date:           |1999-06-09
|State:          |WA
|Lat/Long:       |NA/NA
|Commodity:      |rpp
|**Outcomes**
|Spill volume:   |5475
|Recovered:      |234
|Net loss:       |5241
|Cost:           |4.5e+07
|Cost (USD 1984):|31034279.7330891
|Injuries:       |8
|Fatalities:     |3
|**Causes**
|Cause (self selected):              |OTHER
|Cause (coded by PHMSA):             |all other causes
|Subcause (coded by PHMSA):          |miscellaneous
|System that cause the incident:     |Line Pipe
|Part that caused the incident:      |Pipe
|Year that the part was installed:   |1966
|Year that the part was manufactured:|NA
|**Other impacts**
|Water contamination:                           |NA
|Did a fire occur?                              |TRUE
|Did an explosion occur?                        |FALSE
|Need for surface water remediation anticipated?|NA
|Need for groundwater remediation anticipated?  |NA
|Need for soil remediation anticipated?         |NA
|Need for vegetation remediation anticipated?   |NA
|Need for wildlife remediation anticipated?     |NA

## Resources

### Rupture
[[resources/NTSB_2002_rupture.png|frame,alt=Image of the pipeline rupture on p 41]]
[[resources/NTSB_2002_rupture_2.png|frame,alt=Location of the pipeline rupture as seen on p 43]]

### Spill

> More than 1,200 feet of the creek bed and banks were removed by excavator along the upper portion of Hannah Creek where the creek bed and banks were saturated with gasoline up to 5 feet into the creek face.

[@NTSB2002 p. 54]

> To address additional residual gasoline in surrounding areas that were not excavated, a vapor extraction system was designed and installed with a catalytic oxidation system. The system was completed under the emergency restoration plan, bypassing any
excavated, a vapor extraction system was designed and installed with a catalytic oxidation system. The system was completed under the emergency restoration plan, bypassing any potential permit delays related to construction, and began operation on December 15, 1999. Future efforts will include the operation and maintenance of the systems for several
potential permit delays related to construction, and began operation on December 15, 1999. Future efforts will include the operation and maintenance of the systems for several years until the site is remedied.

[@NTSB2002 p. 55]

### Negligence

> The excavation for the tee did, however, remain open for several days, and although Olympic’s inspector made occasional visits to the site during this time, the inspector made no documented effort to investigate this excavation or question IMCO about it, even though it was only about 100 feet away from the excavation he was reportedly inspecting. In addition, even though Olympic was not notified of the design change that caused the tee to be installed above its pipeline, these changes would certainly have been reflected in the as-built drawings maintained by the contractor at the job site.

## Notes
* Is it that because the computers for the SCADA system were down, the controller did not notice the drop in pressure?
* The leak detection software detects a leak, but the controller started another pump. The pump is eventually stopped after an employee reports gasoline odors [@NTSB2002 p. 7].
* The spill most likely began at 3:28 PM [@NTSB2002 p. 5]. At 4:11PM some operations were resumed [@NTSB2002 p. 7]. At about 4:30PM an emergency response began [@NTSB2002 p. 9]. At 5:02PM the explosion occured.
* 1,890 barrels of the total of 5,638 barrels spilled were lost after the line was restarted. 
* Quick administration test for drugs, but did not test for alcohol because of misscommunication [@NTSB2002 p. 13].
* Description of Olypmics SCADA system [@NTSB2002 p. 15].
* The necessary data would have been available on the SCADE system, but only with extra effort to set up. Nowadays, it would probaby be more easily available, assuming an operator invests in the system. 
* Suspicious repair of coating [@NTSB2002 p. 22].
* Olympic inspectors stating that they were unaware of changes to the construction around the pipeline - for liability reasons?
* In 1996, a smart pig was sent down the pipeline (for magnetic flux inspection), and detected some new anomalies. The inspection company used a wrong formula to calculate the remaining operating pressure (assuming corrosion rather than mechanical damage) and thus did not arrive at the assumption that the damage would reduce the maximum operating pressure [@NTSB2002 p. 26].
* Later, Olpympics was as the result of another spill required to pipelines with a calipter tool. This tool picked up sharp tool damage in the area [@NTSB2002 pp. 27f].
* Olypmic Pipeline failed to carry out an excavation, and the supervising agency failed to notice or enforce the inspection [@NTSB2002 p. 28].
* Some installed valves did not close properly, although I don't understand whether this is by design or not [@NTSB2002 p. 32].
* The pipeline section receivs quite a lot of "false positives", instances where the inlet block valves would close because of high pressure. Potentially normalizing this to controllers [@NTSB2002 pp. 37f]. Hence, these occurances fell through the crack, even though the Olypmic Pipeline's manuals advise a very cautious approach with regard to anomalies [@NTSB2002 p. 39].
* Controllers were often frustrated with the new Bayview products terminal, because of the high workload and stress [@NTSB2002 p. 39]. There was also no specialized training available for the facility [@NTSB2002 p. 40].
* Computer files were missing. The database error claim is inconsistent with independent testing [@NTSB2002 p. 48].
* Ownership of Olypmic Pipelines at the time was split [@NTSB2002 p. 49].
* Corrective action: $3,050,000 civil penalty proposed [@NTSB2002 p. 49]. Corrective action required [@NTSB2002 pp. 76f].
* False positives from smart pigs (magnetic flux inspecteion) [@NTSB2002 p. 60].
* New regulations would have required Olypmic Pipeline to fix the damage [@NTSB2002 p. 61]. But would they have followed up? Does OPS have the resources to put enough pressure on them?
* Wrong pressure relief valve installed [@NTSB2002 p. 67].