# Task 1 – Cyber Security Basics & Attack Surface

## Task Overview
This task is about understanding the basics of cyber security, attack surface, and how data flows in an application.
The goal is to learn core concepts like CIA Triad, types of attackers, OWASP Top 10, and common attack points.



---

## What I Did
- Learned basic cyber security concepts using self-research
- Studied CIA Triad (Confidentiality, Integrity, Availability)
- Researched different types of attackers
- Understood attack surfaces like web apps, mobile apps, APIs, networks, and cloud
- Read about OWASP Top 10 vulnerabilities
- Created a data flow diagram using PlantUML
- Documented everything in simple language

---

## Tools Used
- Browser (Google Chrome)
- Google Search
- OWASP Website
- Cloudflare Learning Pages
- IBM Cyber Security Articles
- VS Code (for PlantUML)
- GitHub


---

## References / Research Links
- https://owasp.org/www-project-top-ten/
- https://owasp.org/www-community/Attack_Surface
- https://www.ibm.com/topics/cybersecurity
- https://www.cloudflare.com/learning/security/
- https://cloud.google.com/learn/what-is-data-integrity

---

## Data Flow Diagram (PlantUML)

```plantuml
@startuml
actor User
participant App
participant Server
database Database

User -> App : Enter data
App -> Server : Send request
Server -> Database : Store / fetch data
Database --> Server : Return data
Server --> App : Response
App --> User : Display result
@enduml
