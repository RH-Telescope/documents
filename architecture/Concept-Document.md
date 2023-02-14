![GitHub Logo](project-telescope-red.png)

## Concept Document

### Problem Space
With more and more organisations utilising OpenShift for their cloud migration/development initiatives, there has been an increased focus on security due to the high exposure of recent system breaches and critical CVEs (Common Vulnerabilities & Exposures).

The majority of organisations already have many security requirements for building, deploying, and maintaining products at scale but it can be hard to achieve observability at the organizational level.
Security policies document what needs to be done, why it needs to be done and how to achieve it whereas governance is the ability to detect if they are being actively applied.  An example is shown below:

* Policy “Why” statement:
  * Using a SAST tool will improve the overall quality of the code developed and reduce risk by identifying possible issues early in the development lifecycle.
* Policy “What” statement:
  * Static Application Security Testing (SAST) must be carried out before an application is deployed to the staging environment.
* Policy “How” statement:
  * Within BigCorp Inc, we recommend using SonarQube or Codacy.

This is a perfectly sensible policy, but assumes that all development teams are aware of it, and able to adhere to it.  

Governance is the ability to demonstrate at a high level that this mandate is being enforced across all development teams.  With these metrics you can further measure risk and take appropriate action if required.

### Objectives

The objective of Project Telescope is to provide this observability in a simple and holistic dashboard, which cuts across all projects and teams to provide a straightforward, standardized binary indication of governance status. Project Telescope also aims to provide a suggestive view regarding quantified risk inherent in projects, based on customer-provided information, Red Hat vulnerability data, and industry best-practice. 

The solution should be tool agnostic with the input streams being received via APIs using a modular plug-in concept.  Examples are plug-ins for Splunk integration, Elasticsearch, Jira plug-in, etc. It is critical that the solution is also extensible for the user, as it is the user's organization which determines the definition of technical compliance as a mandate. 

The dashboard should be capable of displaying data through various lenses.
* Operator Lens: Do these projects adhere to all the relevant mandates? If not, where specifically is the failure?
* Owner Lens:  Do these projects adhere to relevant mandates? How much risk am I exposed to?
* Executive Lens: Are all projects across Platforms adhering to mandate? What about their risk exposure?

Five areas have initially identified which could feed data into the Telescope solution, out-of-the-box:
1. Operations Security
2. Data Security
3. Infrastructure Security
4. Integrations Security
5. Code Security

The MVP won’t initially provide alerting functionality as this will remain the perdue of the organisation’s SIEM solution.

### Outcomes

The main outcome will be to enable DevSecOps teams, Product Owners, and CISOs/CIOs to quickly identify product states of compliance and inherent risk, and allow for better collaboration across multi-functional teams.  Using a plug-in framework will allow development teams to build their own integration points and share them across the organisation.  

The solution should then allow customers to have visibility and reconcile any  deployment of which does not adhere to security mandates, best practices and standards, and also provide strategic alignment of information security focused on their institutional objectives.

It is not intended to be a dashboard which apportions blame to development teams or points fingers at specific individuals but to provide better guidance to teams and provide blameless post-mortems, nor does it seek to gatekeep deployement ability of developers.

The ideal outcome would be for this to be an open source solution with organisations sharing integration plug-ins, bug fixes and creating additional functionality.

A Hackathon was hosted by Red Hat in July 2022 with teams based in both London and North America and an initial dynamic Dashboard was created for the Proof of Concept (PoC).

![Dashboard](dashboard.png)

This shows that Project Telescope is starting to take shape with more development streams planned for the future! 
