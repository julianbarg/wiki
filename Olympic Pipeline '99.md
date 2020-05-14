[[_TOC_]]

Back to [[Oil spills]].

## Incident image

[[https://www.bellinghamherald.com/latest-news/ju0o3y/picture21815628/alternates/LANDSCAPE_1140/Pipeline_smoke.source.prod_affiliate.39.jpg|frame, alt=Incident as seen from the neighborhood, size=600px]] 
  
## Actors 
* [[Olympic Pipe Line]]

## Technology
* [[SCADA]]
* [[RTU]]
* [[PLC]]

## Summary

The pipeline had been damaged in a construction [describe construction]

At the day of the incident, a system administrator entered a faulty data entry into the server that controls the SCADA system. "The system administrator said he noticed that the records [later] contained a typographical error that he said was not there when he created them" [@NTSB2002 p. 11].  This SCADA system is used to remotely control the pipeline. It just so happened that at around the same time, the controller ran a few operations (which were routine operations) on the pipeline via the SCADA system that caused the pressure to spike [@NTSB2002 p. 3]. The pressure spiked to 1,494 psig,; it had previously been tested at 1,820psig [@NTSB2002 p. 14]. Because the system became inoperative at around the same time for about 20-30 minutes, the operator did not notice a sudden drop in pressure at 3:28PM--the burst of the damaged section of the pipeline [@NTSB2002 p. 5]. Thus, later the operator attempt to resume operations, which added another 1,890 barrels bein spilled, leading to a total spill of 5,638 barrels spilled [@NTSB2002 p. 11].

## Significance

Maybe around this time we see the rise of leak detection software. Interestingly, the leak detection software throws an alarm, but the controller seems to ignore it, and starts another pump. Maybe the software still needs to gain legitimacy/authority? Maybe controllers aren't very cautious, or have seen too many false positives/are conditioned to ignore the alarm? Even more interesting is that the pump is later stopped only after another employee smells gasoline odors - a truly unusual occurance [@NTSB p. 7]?

## Learning

### Mechanisms

### Outcomes

## The spill

## Cause analysis

### What could have been done
 
#### To prevent the spill
       
#### To reduce the severity of the spill

### Faulty parts/flawed procedures

## Aftermath/learning
 
## My reactions
* Another incident that the PHMSA did not update on in its database. I can see why the [[commentator|Houston '94##regarding-phmsa-research-and-action]] on [[Houston '94]] as well as the NTSB in general got fed up with the DOT. Assumin that the PHMSA researchers rely on the PHMSA database, it would be fair  assume that they would have a bias toward drawing on data of spills where the cause of the incident is immediately clear and reported in the PHMSA incident report. Fortunately, PHMSA changed their policy starting in 2002 and began to update the database later.
* We continue to see a response that is more focused on discussing the response. Is the message: despite the spill, the deaths should have been avoidable? So is the blame for the injuries put on the rescue personnel instead of the operator? Should rescue personnel be obliged to respon perfectly to an incidents? Is that part of our social contract?

## Various
   
*A story as old as time:  
 
> The system administrator said he noticed that the records now contained a typographical error that he said was not there when he created them. [@NTSB2002 p. 7]

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