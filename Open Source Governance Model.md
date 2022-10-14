# Open Source Governance Model

## Introduction
### Purpose
The purpose of a governance model is to provide guidance on the processes and procedures used within Project Telescope to promote and manage the Open Source Initiative.  This is a living document and will be updated as the Project Telescope team progresses through the initiative with additional processes and procedures being added and updated as maturity increases.

This document will allow for better management of the upstream Open Source project and provide a framework for its use.

### Goals
There are a number of goals which drive the content of this document.  
These are:
- Provide a high level overview of the project goals and potential development phases.
- Decentralise the development process by allowing developers from each geo/region to develop the code base as a community.
- Deliver consistently high quality software throughout the project.
- Increase awareness and adoption of the Project Telescope within both Red Hat, our partners and our customers.
- Provide guidance and policies to all participants of the initiative.
- Identify lead maintainers and contact details.
- Identify various roles for contributors, maintainers and other users.
- Document release frequency, release conventions and tooling.

## Adopting a “Do-ocracy”
Project Telescope is a relatively new open source project with contributors across various Red Hat geos and teams.  To enable a simple, workable and outcome based environment, a “do-ocracy” is planned to be the initial governance model.

Open source projects adopting the do-ocracy governance model tend to forgo formal and elaborate governance conventions and instead insist that decisions are made by those who do the work. In other words, members of a do-ocracy gain authority by making the most consistent contributions. Peer review remains common under this model, but individual contributors tend to retain de facto decision-making power over project components on which they have worked most closely.

For this reason, some do-ocracies will claim they have no governance at all, relying instead on individual stakeholders' authority to make decisions on matters where they have done the most work. But such claims about an absence of governance are misguided. Every open source project has a governance model. In the case of most do-ocracies, the governance model is merely implicit in the everyday interactions of project members. As a result, joining them can be difficult and intimidating for newcomers, as would-be contributors might not immediately know how to participate or seek approval for their contributions.


## Project Overview
Increasingly, organisations find that transformative digital adoption and a growing requirement for security are diametrically opposed, and they are unable to ensure even minimum viable security is effective. This is due to a combination of their inability to keep pace with the scale and speed of modern development, and a reliance on legacy governance mechanisms.

We have ideated and begun architecting a capability called Project Telescope, which would allow us to automate cyber security governance across disparate ecosystems in a vendor agnostic way. This capability will allow customers to more accurately and rapidly mandate security requirements, visualise compliance to said mandate in real-time, reduce time to go-live for new product development, and enhance security and risk management both at the product development and leadership levels.

The project will aim to focus on 5 specific domains but the aim is for it to be extensible so customers can add their own domains which are relevant to their specific needs.

1. Logging & Monitoring Security
2. Data Security
3. Infrastructure Security
4. Code Security
5. Integration Security

Each domain will have a simple “Why, What and How” definition to explain the requirements at a high level.  Customers will have the ability to add their own definition which meet their security compliance requirements.  Some examples are shown below:

### Code Security
| Why | What | How |
|-----|------|-----|
| Using a SAST tool will improve the overall quality of the code developed and reduce risk by identifying possible issues early in the development lifecycle. | Static Application Security Testing (SAST) must be carried out before an application is deployed to the staging. environment. | Within BigCorp Inc, we recommend using SonarQube or Codacy. |

### Image Security
| Why | What | How |
|-----|------|-----|
| Private image repositories can enforce image signing so only signed images are pushed and used in a given environment.  This can help reduce risk and ensure that only trusted and verified images are used across the organisation. | All base images should be stored in a recognised, certified and protected image registry. | Within BigCorp Inc, we recommend Red Hat Quay for storing all base images. |

### Logging Security
| Why | What | How |
|-----|------|-----|
| Security monitoring and logging is central to the identification and detection of threats to your IT systems. It acts as your eyes and ears when detecting and recovering from security incidents. Effective monitoring relies on proportionate, reliable logging and device management practices.  | The following logging should be forwarded to a centralised logging system: Host-based logs, Service logs, Infrastructure logs, System compliance audits  | Within BigCorp Inc, we recommend that all logs are forwarded to our centralised Splunk instance. |

## Project Roles
Project Telescope will have a variety of real roles, but only a handful need to be defined to start out as we will begin with a do-ocracy. Those basic roles to be agreed are are:

### Member
This is possibly the least-documented role in open source projects, despite being the most pervasive. Members are the people or organisations who participate in the project and are recognized for it. Depending on how the project is run, these can be subscribers on a mailing list, sponsoring companies, known end-users, participants at an event, or members of a foundation. In some projects, Member is synonymous with Contributor, but this is not always the case. Most projects have a much larger group of people who are involved with the project in some way but are not actively contributing code or content to it.

Defining who Members are requires deciding who the project is actually serving, which is always a critical discussion to have. Are customers of the main sponsoring company automatically project Members? Can companies be Members, or only individuals? Are end-users Members or can they only be contributors be Members? More than anything, defining Members means defining to whom it is that project Leaders need to listen.
For almost all projects,specify what rules Members are subject to (usually a code of conduct and not much else) and what they can expect from Leaders and Contributors. It’s particularly helpful to explain how Members should participate in the project, such as "Members file bugs against this repository, and use the 'new bug' template." Most people, given clear instructions, are happy to channel their participation into the routes shown to them.

### Contributor
Far more projects have a written definition of Contributors, but fewer than one might expect. It’s often assumed, in the age of publicly hosted source code control, that anyone in the GitHub or GitLab statistics are counted as Contributors. But defining "who is a Contributor to this project" can be deceptively hard.

Is it anyone who posted on a mailing list, or does one need 100 merged pull requests to qualify?
Is it just code contributors, or contributors of any kind? What about folks who do events and advocacy? Are staff who work for a contributing company automatically considered Contributors, or do they have to earn it individually? What about someone who contributed a lot of code three years ago, but not since then? Who gets listed in project release credits and how?

The Contributor role is also one for which many more expectations will need to be set for what Contributors receive in return for their work. This not only includes an explanation of the intellectual property rules of the project (e.g., does the contributor still own their code), but also questions like how soon Contributor can expect their submissions to be reviewed and accepted or rejected. Generally, how the Contributor will be credited for their participation should also be explained.

### Leader
As noted, every project has leadership, even when those leaders are not clearly identified. As such, at a minimum it will be necessary to transparently identify who the Leaders are, so that decision-making processes can be clear. Many projects also explain the qualifications and procedure to become a Leader, whether it’s selection by a committee, election, or simply based on a specific job. If working in a more politically sophisticated project, then those should be written down in a selection/election procedure document, but if it’s simple, selection can just be part of the role document.

What fewer projects put into their leadership role documents are the other parts: the powers and limitations of the Leaders, their duties, and how people leave the role (voluntary or otherwise). It’s very important that everyone knows exactly how far a Leader’s authority extends, as well as what they’re responsible for, or a project will end up with a lot of conflict between Leaders and other project members. Having a set of written duties helps immensely when a leadership team has to decide to remove a project Leader who has stopped participating, but does not want to resign.
If a project is trying to recruit new/additional Leaders, then it’s also important to have a detailed set of qualifications a Leader needs to meet. Contrary to some expectations, having detailed qualifications gives people who want to move up in the project a goal to aim for.

## Contributor Covenant Code of Conduct
Our Pledge

"We as members, contributors, and leaders pledge to make participation in our community a harassment-free experience for everyone, regardless of age, body size, visible or invisible disability, ethnicity, sex characteristics, gender identity and expression, level of experience, education, socio-economic status, nationality, personal appearance, race, caste, color, religion, or sexual identity and orientation.  We pledge to act and interact in ways that contribute to an open, welcoming, diverse, inclusive, and healthy community."

Standard CoCo documents added at: https://github.com/RH-Telescope/documents/blob/main/CODE_OF_CONDUCT.md


## Policies and Procedures (P&Ps)
In addition to some basic role documentation, there’s a certain amount of basic paperwork that each project should create for itself. These policy and procedure (P&P) documents are considered a kind of minimum for what a community needs in order to grow and mature a project.

A project may, and eventually will, have other P&P docs as its contributor base expands and the number of processes needed to write down will expand as well.
Some of these will be mostly technical (like release process, or a support policy), and we won’t be exploring those here.

However, there are three minimum governance P&P that every project should have:
- Code of conduct
- Contribution process
- Communication information

## Open Source Repositories
https://github.com/RH-Telescope

## Open Source License
TBC
