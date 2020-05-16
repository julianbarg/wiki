[[_TOC_]]

Back to [[Oil spills]].

## Incident image
[[https://bloximages.chicago2.vip.townnews.com/theeagle.com/content/tncms/assets/v3/editorial/e/cc/eccb11ba-019b-11e2-a931-0019bb2963f4/50588327704e9.image.jpg|alt=Aftermath of the explosion, frame, width=600px]]

## Documents

### NTSB report
* [[https://www.ntsb.gov/investigations/AccidentReports/Reports/PAR9301.pdf]]

### News reports
* Local news: [[Salt dome explosion: 20 years later|https://www.theeagle.com/townnews/commerce/salt-dome-explosion-20-years-later/article_cab6128c-019b-11e2-8e7e-0019bb2963f4.html]]
* NYT: [[Gas Explosion Tears Through Texas Pastures|https://www.nytimes.com./1992/04/08/us/gas-explosion-tears-through-texas-pastures.html]]

### Videos
* News report: [[https://youtu.be/IpYIvyCXv9w]]

## Actors
* [[NTSB]]
* Operator of the pipeine: Seminole Pipeline Company. Largest shareholder at the time was [[MAPCO]], the pipeline (and its operating company) is currently owned by Enterprise Products Operating.
* Research and Special Programs Administration ([[RSPA]]) of the [[DOT]], [[OPS]] 
* [[FERC]]
* Texas Railroad Commission ([[TRC]]) 

## Significance

Regulators and industry organizations largely have not recognized the potential risk that stems from misoperated storage caverns [@NTSB1993 pp. 54f]. Could a significant takeaway from the incident be as simple as "hey, look, these things can blow up, too"? For instance, the [[AGA]] believed that the gas, if leaking, would simply dissipate quickly and hence not pose a hazard [@NTSB1993 p. 56].

The report also features a great section that gives an idea of how organizational memory might be encapsulated in routines [@NTSB1993 pp. 24ff]. See e.g., [[resources|Seminole '92#organizational-memory]], further [@NTSB1993 p. 34]. The lack of written rules to follow is partially blamed for the failure. On the one hand, math errors could certainly be corrected - that would help [@NTSB1993 pp. 31f]. On the other hand, when written rules exist, it may then be flaws in written rules that are blamed for failures? Maybe as a result of the flawed organization of memory, the dispatcher made the fatal mistake of reopening the pipeline valves to the salt dome [@NTSB1993 pp. 38]. See also [[notes|Seminole '92#The-valve-opening]].

### Learning

#### Mechanisms
* More complex SCADA systems to display e.g., historical data in a chart, separate output for individual sensors.
* Attention drawn to storage caverns - leading to new regulation.
* Problems with training and procedures at MAPCO.
* Fail safe equipment.
* System safety analysis.
* Emergency procedures - both for local employees and EMS etc.

#### Outcomes
* Lower failure rate for storage caverns.
* Detection of more failure for storage caverns.
* Less injuries and fatalities from failures of storage caverns.

### Other

## Summary

The Brenham station is a salt cavern that is used as part of the MAPCO pipeline network for interim storage of HVLs. Since it is a "natural" structure of flushed out salt that is expending with operations, its capacity is only known when it is measured (which happens every couple of weeks). The [[NTBS]] later determined that in the weeks leading up to the incident, the cavern was filled over capacity at several points in time. The cavern was over capacity because the employees made errors when calculating the volume of HVL that was pumped into the cavern [@NTSB1993 p. 31]. The employees did not know exactly how to calculate the volume because they did not have a relevant educational background and did not receive appropriate guidance [@NTSB1993 pp. 25f]. The employees that later arrived on site did know how to determine whether the cavern was overflowing, and how to shut off the flow of HVL into the cavern. When the cavern was already overflowing, the remote dispatcher first did not recognize the emergency [@NTSB1993 pp. 59f] and later used the [[SCADA]] system to close the valve to the cavern. At this point, a "large mushroom-shaped cloud" was already visible over the station and the area had been foggy for at least 20 minutes [@NTSB1993 p. 39 and pp. 100f]. Later, he was worried that too much pressure on the connecting pipeline might be an issue, so he reopened the valve - in reality, the pipeline would have shut down automatically once it reaches a certain pressure [@NTSB1993 p. 38].

## The spill

The overflowing gas covered the surrounding area in a haze. An employee parked on the access road and stopped on driver from entering the area. Another driver however bypassed the vehicles and entered the fog. Soon after that vehicle entered, an explosion occured that leveled a large area, including

## Cause analysis

A core issue is that Y-grade HVL did unexpectedly escape through the brine, thus keeping pressure inside the cavern constant and masking the emergency.

* Two valves in a sensing line, which could have prevented the spill by automatically shutting flow to the facility, had erroneously been manually closed. It could not be determined when or by whom [@NTSB1993 p. 60]. Thus, a wellhead safety system was inoperative [@NTSB1993 p. 60].
* Information displayed on the SCADA system were incomplete, did not show historic data and thus trends [@NTSB1993 p. 61].
* The HAZGAS detectors only send a single signal, even if multiple of them went off.
* A lack of communication between employees [@NTSB1993 p. 72].
* Existing regulations did not apply to HVL underground storage facilities [@NTSB1993 pp. 81f].
* Lacking procedures and training.

### What could have been done

#### To prevent the spill
* Failsafe safety system
* Correct accounting of HVL volume

#### To reduce the severity of the spill
* Show historical data on SCADA
* Employees could have realized severity of the situation sooner, and contacted local emergency personnel

### Faulty parts/flawed procedures
* Training and lack of procedures for emergencies.

## Aftermath/learning
* MAPCO replaced the SCADA system "to graphically display both historical and current operational data on all boards at the dispatch center" [@NTSB1993 p. 62].
* Added a meter to a previously unmetered valve from the cavern to a mainline [@NTSB1993 p. 69], which results in a complete picture of volume in the cavern (all inputs and all outputs). MAPCO will upgrade all other storage caverns in their system similarly [@NTSB1993 p. 71].
* MAPCO established a training excercise with public response agencies [@NTSB1993 p. 81].
* MAPCO installed a siren at the station that can be activated by the sheriff's office [@NTSB1993 p. 81].
* The station will also be manned 24/7 from now on [@NTSB1993 p. 81].
* Texas Railroad Commission ([[TRC]]) prepared to more regulation [@NTSB1993 p. 84].

## My reactions
* Maybe I should adjust my expectations. If we could stop chemical plants and other facilities in Texas from randomly exploding all the time, that would already be a relatively great achievement. Move the goalpost. Overall though - let's not generalize. Learning is possible if intentionally pursued.
* Interesting insights into how organizational memory works [@NTSB1993 pp. 25f.]. One can immediately imagine how an understanding of the system may gradually get lost in this game of telephone. Clear lack of documentation. See also [[resources|Seminole '92#organizational-memory]].
* Today, a word file or simple script would probably be used to calculate the inflow and outflow of HVL into the salt dome. Which may also leave room for error given a lack of understanding? But less likely? Would that be learning? The fact that an excel file would be created? Or just a switch in routines? Is switching routines learning? Wouldn't the best approach be to have somebody at the job who actually understands the process that is going on? Is it learning if we manage to allow for an untrained person to do the job of a trained person, even if this increases risk, because it is more efficient?
* Is this an operator error? Or a hiring issue? Or a training issue?
* Everything has to explode once in order for us to recognize it as a potential safety hazard? Is learning from failure really that simple?

## Various
* "He stopped his truck a short distance before the swale and turned the ignition switch off. He said that when the pickup continued to run, 'I knew something serious had happened" because "there was enough gas in the air to keep feeding my engine.'" [@NTSB1993 p. 4].

## Data

### PHMSA narrative

"((Death and injury information based upon media reports)).  An explosion and fire occurred in the area around seminole pipeline company's brenham station.  This incident is currently under investigation by the national transportation safety board to determine the cause."

### Quantitative data

|**General information**
|----------------|---:
|Incident ID:    |19920109
|Operator name:  |Seminole Pipeline
|Date:           |1992-04-06
|State:          |TX
|Lat/Long:       |NA/NA
|Commodity:      |hvl
|**Outcomes**
|Spill volume:   |0
|Recovered:      |0
|Net loss:       |0
|Cost:           |0
|Cost (USD 1984):|0
|Injuries:       |20
|Fatalities:     |3
|**Causes**
|Cause (self selected):              |OTHER
|Cause (coded by PHMSA):             |all other causes
|Subcause (coded by PHMSA):          |miscellaneous
|System that cause the incident:     |No Data
|Part that caused the incident:      |No Data
|Year that the part was installed:   |1982
|Year that the part was manufactured:|NA
|**Other impacts**
|Water contamination:                           |NA
|Did a fire occur?                              |TRUE
|Did an explosion occur?                        |TRUE
|Need for surface water remediation anticipated?|NA
|Need for groundwater remediation anticipated?  |NA
|Need for soil remediation anticipated?         |NA
|Need for vegetation remediation anticipated?   |NA
|Need for wildlife remediation anticipated?     |NA

## Resources

### Scada limitations

[[resources/NTSB_1993_scada.png|frame, alt=Flaws of the scada described on page 19,width=600px]]

### Organizational memory

[[resources/NTSB_1993_memory.png|frame, width=600px, alt=Flaws of organizational memeory on pages 25f]]

### Previous releases

[[resources/NTSB_1993_previous_releases.png|frame, width=600px, alt=Previous relaeses described on page 50]]

## Notes
* Flawed safety system, see also [[here|Seminole '92#Scada-limitations]].
* Disaster could have been much, much greater [see @NTSB1993 pp. 7f].
* The company did not have exact data on the gas going in and out [@NTSB1993 pp. 31].
* Personnel did not receive formal instructions for carrying out the calculations for inflow and outflow of HVL [@NTSB1993 p. 25].
* The facility was supposed to be designed to automatically deal with failure [@NTSB1993 p. 26].
* No written guidelines on many functions of the facility [@NTSB1993 p. 34].
* "He was not aware that the plant pumps were designed to shut down automatically when the pump pressure increased to 1,550 psig" [@NTSB1993 p. 38].
* Extend of public education [@NTSB1993 pp. 42f].
* Cavern storage not regulated more strictly because as part of pipeline systems, they kind of fell throught the cracks [@NTSB1993 p. 51].
* Before the incident, an industry association ([[AGA]]) held that storage systems such as the one involved in this accident were universally save [@NTSB1993 p. 56].
* Summary on training [@NTSB1993 p. 73].
* Again a feud with the RSPA [@NTSB1993 pp. 75f].

### The valve opening
* "The other dispatchers were able to contact personnel at one of the two plants pumping into the Bryan Lateral and have them shut down operations almost immediately. However, when they could not get anyone to answerat the second plant, the dispatcher at the Seminole board became apprehensive that if a plant continued to pump product against a closed valve, the pressure might rupture the lateral, so he reopened the Bryan Lateral. He was not aware that the plant pumps were designed to shut down automatically when the pump pressure increased to 1,550 psig" [@NTSB1993 p. 38].