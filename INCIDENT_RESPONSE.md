# 1 - INCIDENT RESPONSE OVERVIEW
## WHY ORGANISATION SHOULLD HAVE AN INCIDENT RESPONSE PLAN
All organisations have risk associated with infosec and data privacy and raliability
A good I.R plan can reduce the impact and cost of a cybersec incident
So it supports responding to incident systematically so that appropriate actions are taken.
## Phases that makes up an incident response
* Preparation
* Detection
* Analysis
* Containment
* Eradication
* Recovery
## DEFINING AN INCIDENT 
* **Event** : Something that hapened in inf sys but nothing malicious or requiring actions EX: login
* **Alert** : Notification from IDS, IPS having a malware ....
* **INCIDENT (small i )** : Violation of CIA without a buissness impact
* **INCIDENT (capital I )** : Violation of CIA with a buissnes impact
* **Breach** : Loss of specific data that triggers legal obligations above and beyond I.R
## SECURITY OPERATIONS CENTER
![net](https://www.exabeam.com/wp-content/uploads/2018/08/soc-graph@3x.png)
## CERT ( CYBER INCIDENT RESPONSE TEAM )
* **Central** : As a small company who have their team in the same local
* **Distributed** : A large company who have multiple locals and evey local have his own I.R team
* **Coordinating** : An freelancer or a separated company who response to incidents for other company's
## CERT
+ CIRT can range  >= 1 person
+ May be on premise or virtual or a combination
+ May be 24x7 or just during working hours
## CERT COMMUN SKILL SETS
+ Threat intelligence
+ Network Forensics
+ Threat Hunting
+ Scripting & coding
+ Digital forensics
+ Malware reverse engineering
## I.R TEAM ACCESS
+ What privilleged accounts do I.R team need ?
	Should they see the config file from routers & switches , read firewall ....
+ Does the I.R team need access to apps, sys, db, Net devices, etc... ?
+ How is the I.R team access to systems monitored ?
	Who's watching the watchers, capturing the activity's
## QUESTIONS TO ASK DURING AN INCIDENT
**1**- Now what ?
**2**- Who should i report it to ? and what should i report ?
**3**- how mush will this cost ?
**4**- what this the attackers take ?
**5**- how did dey get in ?
**6**- what will it take us to get back to full operations ?
**7**- what else we don't know about ?
**8**- how could we have prevented this ? & how do we make sure it never happens again ?
**9**- how could we have been better prepared ?
**10**- who were the attackers ? & what was their motivation ?
## COMMUN STAKEHOLDERS FOR I.R
+ Chief Executive
+ Human Resources
+ Information Technology
+ Board of Respnsables
+ Customers / Clients
+ Communication / public affair
+ Legal
+ Auditors
## SOC TEAM & I.R
+ Its not advisable to have I.R complitlly with SOC , cuz montoring may stop during an incident
+ Its good to have cross-tranning between the Two to shre knowledge
+ If there is only one person for I.R he must focus on updates, good I.R plan, outside agents
# 2 - INCIDENT RESPONSE PROCESS
## PREPARATION
The incident response process includes identifying an attack, understanding its severity and prioritizing it, investigating and mitigating the attack, restoring operations, and taking action to ensure it won’t recur.
An incident response plan (IRP) is a set of documented procedures detailing the steps that should be taken in each phase of incident response. It should include guidelines for roles and responsibilities, communication plans, and standardized response protocols.
Here are the main reasons you must have a strong incident response plan in place:
### Prepares you for emergency
security incidents happen without warning, so it’s essential to prepare a process ahead of time
### Repeatable process
without an incident response plan, teams cannot respond in a repeatable manner or prioritize their time
### Coordination
in large organizations, it can be hard to keep everyone in the loop during a crisis. An incident response process can help achieve this
### Exposes gaps
in mid-sized organizations with limited staff or limited technical maturity, an incident response plan exposes obvious gaps in the security process or tooling which can be addressed before a crisis occurs
Preserves critical knowledge
an incident response plan ensures critical knowledge and best practices for dealing with a crisis are not forgotten over time and lessons learned are incrementally added
Practice makes perfect
an incident response plan creates a clear, repeatable process that is followed in every incident, improving coordination and effectiveness of response over time
## DETECTION & ANALYSIS
### PRECURSORS
A precursor is a sign that an incident may accur in he future so you get a heads up
For example : could be a web server log entries that show an usage of a vulnerability scanner
An announcement of a new exploit that targets a vulnerability of an organization's
A group stating that the said group will attack the organization.
### INDICATORS
An indicator is a sign that an incident may have accured or accuring in the moment, present
For example : Antivirus notifications that a host is infected with malware
A system admin sees a filename with unusual caracters (ransomeware)
Emails sent to employees with suspicious content
### MONITORING SOFTWARES
+ INTRUSION DETECTION / PREVENTION SYSTEM
+ DLP DATA LOSS PREVENTION
To ensure that sensitive data is not lost, misused, or accessed by unauthorized users
+ SIEM
Deals with the log files directly to create an event or an alert
## CONTAINEMENT
Containment is important before an incident overwhelms resources or increases in damage. Containment strategies vary based on the type of incident. The whole point of containment is to be able to stop the threat and mitigate any further damage.
## ERADICATION
Eradication os the process of getting rid of the incident, deleting the malware, securing the ports, block the users ...
## RECOVERY
Recovery may involve such actions as restoring systems from clean backups, rebuilding systems from scratch, replacing compromised files with clean versions, installing patches, changing passwords, configuring the network, such as the firewall rulesets, router access control lists, etc.
# 3 - INCIDENT RESPONSE DEMO
## QRADAR
 Qradar is a SEIM tool which collect logs with the capability's to search, detect and alert. Qradar collect informations from apps, ids/ips , next gen firewall, and others . 
After Qradar collect the infos, Qradar process the data collected and analyse it using a set of rules .
## Incident Response process Bassed on SanS :
### Preparation : 
Preparation is the gatheding of infos so you can response to an incident, infos could be list of assets, I.R plan, tools, contacts, stakeholders ...
### Detection and analysis :
Begins with an alert recieved , next gathering as much data possible about the alert so you can investigate it. After the information is gathered, we will start analyzing the data gathered to determine the entry point, footprint and validity of the alert.
### Containment, eradication and recovery :
after the entry point is identified, you nedd to contain the threat to stop it from cauzing more damage, after that you need to work on removing the threat, by fixing the vulnerability's, reseting the configuration, restoring backups ... so that you can restore the system to his normal state .
