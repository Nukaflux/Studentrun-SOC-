### Mitchell C. Hill Student Run SOC Documentation

![](https://github.com/Nukaflux/Studentrun-SOC-/blob/master/unnamed.png?raw=true)



### About me
Hello my name is Jensen and I am currently working on projects at the Mitchell C. Hill Student Data Center. Specifically at the Security Operations Center. I am currently a fourth year studying cyber security and hope that my projects here help you out! I specialize in the use of Splunk Enterprise, a powerful data analytics platform that can also be deployed as a SIEM.

### About the Student Run SOC

The student run SOC at Cal Poly Pomona is project that students can utilize in the near future. SIEMS (Security information and event management) are used in the industry to protect and monitor businesses. The student run SOC will run 3 SIEMS, those being IBM Q-radar, Splunk enterprise, and LogRhythm. Students will get to use the 3 industry standard SIEMS to gain insight and hands on exprience in security operations. The SOC will provide real-time analysis of security alerts generated by applications and network hardware.

### What is here?
I currently will be posting copies of my search queries. These search queries are directly from splunk enterprise and can be applied in your own siem instance of Splunk. Splunk developed the Search Processing Language (SPL) to use with Splunk software. SPL encompasses all the search commands and their functions, arguments, and clauses. One way to learn the SPL language is by using the Search Assistant. This is where I will store SPL specific files. 


### SIEM Concepts and processes:

	A SIEM can be compared to a complex machine in that a SIEM has several moving parts, each performing a specific job, that need to work properly together or else the entire system will fail. There are variations on the standard SIEM, with additional specific parts, but a simple SIEM can be broken down into seven separate pieces or processes. Understanding this will allow you to under Splunk’s SIEM processes. 


### Source Device>Log Collection>Parsing>Correlation>Log Storage+Rules>Monitoring



•	The source device is a device that feeds information into the SIEM. A source device is the device, application, or some other type of data that you want to retrieve logs from that you then store and process in your SIEM.

•	The next step in the device or application log flow is to somehow get all these different logs from their native devices to the SIEM. This Log Collection.

•	Next after the data is being forwarded to the SIEM what happens? You need to Parse the data in useable data. Lucky for us Splunk automatically categorizes data into sources, event type, and field. 

•	Now comes correlation. You investigate the logs and find a pattern. You might notice that a sequence of more than 200 of the same events has occurred in the past 1 minute. That would raise suspension. 

•	After having suspension, you save the log, and apply rules and logic. An example would be “If there more than 100 or more failed authentications from the same source, an alert will be sent. This is the power of log storage and rules used in parallel. I have applied this logic for a possible brute force alert in our own SOC. 

•	Monitoring, then comes into play. With preconfigured alerts and reports, SOC Analysts can then report the incident to a SOC Manager and Security Architect. The issue is reported, investigated, and resolved. 
