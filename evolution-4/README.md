# Evolution 4: Networking and Cybersecurity Competency Assessment

**Oscar Garza | CIDM 6340 and CIDM 5380 (in progress)**

## Current preparedness

My preparation in Networking and Cybersecurity combines practical security assessment with the responsibilities of developing software for a financial-services organization. CIDM 6340, Network Management and Information Security, strengthened my ability to investigate exposure, interpret findings, and communicate improvements. CIDM 5380, Cloud Computing and Security, is extending that foundation into cloud infrastructure and application communication. This assessment reflects my completed networking coursework and the cloud knowledge and practical skills I have developed so far.

Building on my [Evolution 0 assessment](../evolution-0/README.md), I am confident investigating exposed systems and services, evaluating potential vulnerabilities, configuring access controls, and participating in a formal security audit. I am also prepared to assist with authorized penetration testing, although my strongest portfolio evidence is a baseline security assessment. My principal growth areas are cloud networking and maintaining secure configurations as systems and dependencies change.

## What I know: evaluating security in context

My most representative artifact is the [final security audit for The Isaac Apartments](https://github.com/oegarza1/6340-networking-assignments/blob/main/Assignment6/Oscar_Garza_The_Isaac_Security_Audit_Report.pdf). It brought together skills developed in earlier assignments and applied them to an operational environment. Using a completed audit plan, I reviewed network exposure, workstation controls, cloud-based business systems, physical security, and staff procedures. The report explicitly describes a practical baseline review rather than a full penetration test or forensic investigation. That scope is important when explaining what the findings establish.

The audit recorded eleven passing items out of sixteen, with five items that did not fully pass. A ShieldsUP check did not identify open ports among the external services tested, but the broader review identified weaknesses that a port scan alone would not reveal. These included inconsistent workstation locking, shared local access, and the absence of a written local incident-response plan. Cloud storage or retention appeared to provide some backup capability, but staff could not demonstrate a documented restore process. The resulting assessment described a moderate risk posture with practical opportunities for improvement.

This work was meaningful because it revealed the difference between having some protections and being prepared to respond when those protections fail. The apartment staff had informal ideas about whom to contact, but recovery procedures and responsibilities were not sufficiently documented. My recommendations included automatic screen locking, named accounts, access reviews, a device inventory, a short incident checklist, and periodic restore testing. These were proposed improvements; the audit does not establish that they were subsequently implemented. My contribution was to turn observations into an actionable account of risk and preparedness.

The [supporting networking portfolio](https://github.com/oegarza1/6340-networking-assignments) also contains network-design work, Nmap mapping, Wireshark analysis, vulnerability scanning, and a ransomware recovery plan. The final audit integrates these areas by connecting technical observations to operational consequences. It demonstrates my ability to explain why a quiet external network boundary does not eliminate risks associated with credentials, unattended workstations, or unclear recovery responsibilities.

## Cloud foundations and application communication

In CIDM 5380, I have studied Linux and cloud foundations; DNS, reverse proxies, firewalls, and HTTP/HTTPS; database persistence and access control; FastAPI communication; and monolithic and decoupled architectures. My hands-on experience includes working with databases on Google Cloud and configuring the access needed to modify them. This reinforces my understanding that a working connection must also have an appropriate permission boundary.

My [cloud web-app repository](https://github.com/oegarza1/5380-cloud-computing) provides concrete implementation evidence. The monolithic application queries SQLite and renders HTML through one service. The decoupled version separates a static frontend from a FastAPI backend that retrieves grades through an API. This separation makes service communication and browser access settings visible parts of the design. The backend also uses a parameterized database query, demonstrating a specific defensive coding practice.

These applications are instructional examples. The decoupled backend permits requests from any origin and has no authentication or authorization layer. They therefore demonstrate communication and architectural foundations, while also illustrating controls that would need further work before handling protected information. I look forward to extending this foundation through further coursework in Docker, CI/CD, orchestration, and observability.

## Professional application and areas for growth

Security is a routine part of my payment-platform responsibilities. Access to live production data is restricted, including access by developers such as myself. On the application team, I work to mask sensitive information in logs while preserving enough diagnostic context to investigate failures. I also help maintain current libraries that meet firm requirements. These practices connect least privilege and data protection to everyday engineering decisions: the information useful for troubleshooting must be balanced against what a person or service is permitted to see.

One of my most important learning experiences has been distinguishing an informational observation from a vulnerability that requires action. When many findings appear threatening, established assessment resources and tool explanations help organize the investigation. OWASP-related guidance has been part of that learning, but a label or severity assessment still requires interpretation in the context of the affected system. I need to consider exposure, existing controls, and business consequences before deciding what deserves priority. The apartment audit reinforced this judgment by identifying process weaknesses even where the external scan showed limited exposure.

I want deeper practical understanding of cloud networking and greater consistency in maintaining secure configurations. I can apply access controls, but I want to become more independent when tracing how traffic reaches a service and determining where restrictions should be enforced. Configuration maintenance also requires understanding whether a change weakens a previously established control. Potential gaps I should investigate include configuration drift, the division of responsibility between cloud providers and application teams, and how to verify that protections remain effective after deployment. These extend the maintenance concerns identified in my [Software and Systems assessment](../evolution-3/README.md).

## Learning resources and continued development

Google Cloud labs and DataCamp have been useful learning resources. The labs provide hands-on opportunities to apply concepts, while DataCamp instruction helps me prepare for the practical exercises. Course materials, the audit plan, and the resulting reports give me a structure for connecting those activities to evidence.

The linked repositories provide work samples that connect my learning to practical application. Reviewing these artifacts helps me assess what I can demonstrate independently and where I still need further practice.

## Integration and capstone readiness

Networking and Cybersecurity connects the other curricular areas by protecting the systems and information on which their results depend. Data Management defines which records exist and how access is structured. Software Systems implements the workflows and permission checks that use those records. Data Analytics can identify operational patterns, but its datasets and logs must also be protected from inappropriate access or disclosure. My professional work makes these relationships concrete whenever an API handles sensitive information or produces diagnostic events.

My capstone direction remains tentative, with Java and AWS still my preferred foundation. I would like to demonstrate authorization for selected APIs, redacted logs, and maintained security configurations. A prototype could make these controls reviewable through allowed and denied requests, synthetic diagnostic events, and documented configuration checks. The portfolio would connect implementation evidence to the audit skills developed in CIDM 6340, while the presentation would explain the protected workflow and its limitations.

I am prepared to contribute access-control implementation, contextual assessment of findings, and clear communication of security improvements. My integrated capability is to build services that organize data, support analysis, and make protection and operational preparedness part of the design. Continued work in cloud networking and configuration maintenance will help me sustain those protections as the system evolves.
