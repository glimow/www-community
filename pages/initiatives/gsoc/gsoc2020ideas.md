---

layout: full-width
title: GSoC 2020 Ideas
tags: gsoc
permalink: /initiatives/gsoc/gsoc2020ideas

---
# GSoC2020 Ideas
<!-- Template: Use a format like below to add your project:
### [Project Name]

##### [Explanation of Ideas]

##### [Expected Results]

##### [Getting Started]

##### [Mentors]
-->

## OWASP Project Requests

Tips to get you started in no particular order:
- Read the [Student Guidelines](gsoc2020).
- Contact us through the mailing list or irc channel.
- Check our [github organization](https://github.com/OWASP).

## List of Project Ideas

### [OWASP Python Honeypot](https://github.com/zdresearch/OWASP-Honeypot)

##### Explanation of Ideas

OWASP Honeypot is an open source software in Python language which designed for creating honeypot and honeynet in an easy and secure way! This project is compatible with Python 2.x and 3.x and tested on Windows, Mac OS X and Linux.

##### Expected Results

* Zero Bugs: Currently we may have several bugs in different conditions, and it's best to test the all functions and fix them
* New modules: add some creative ICS/Network/Web modules andvulnerable web applications, services and stuff
* API: update API sync to all features
* WebUI: Demonstrate and add API on WebUI and Live version with all features
* WebUI Special Reports: Track the attacks more creative and provide high risk IPs
* Database: Better database structure, faster and use queue
* Data analysis: Analysis stored data and attack signatures
* OWASP Top 10: Preparing useful processed/raw data for OWASP top 10 project

##### Getting Started

It's best to start from GitHub [wiki page](https://github.com/zdresearch/OWASP-Honeypot/wiki), we are looking forward to adding more modules and optimize the core.

##### Students Requirements

* Python
* Packet Analysis & Tshark & Libpcap
* Docker
* Database
* Web Development Skills
* Honeypot and Deception knowledge

##### Mentors
* [Ali Razmjoo](mailto:ali.razmjoo@owasp.org)

### [Zed Attack Proxy (ZAP)](https://www.zaproxy.org)

#### Idea One: GraphQL Support

ZAP does not currently detect [GraphQL weaknesses](https://github.com/zaproxy/zaproxy/issues/5153) such as injection, auth problems, or information exposures.

##### Expected Results

* Implement functionality to allow ZAP to inspect and attack given GraphQL endpoints.
* Code that conforms to our Development Rules and Guidelines

##### Getting Started

* Have a look at the ZAP [CONTRIBUTING](https://github.com/zaproxy/zaproxy/blob/develop/CONTRIBUTING.md) guideline, especially the 'Coding' section.
* We like to see students who have already contributed to ZAP, so try fixing one of the bugs flagged as [IdealFirstBug](https://github.com/zaproxy/zaproxy/labels/IdealFirstBug).

##### Mentors
* [Simon Bennetts](mailto:psiinon@gmail.com) and the ZAP core team.

#### Idea Two: SSRF Detection/Handling

ZAP is currently able to detect vulnerabilities with limited local network callback support (such as XXE).
ZAP could benefit from enhanced callback support in the form of a configurable or deployable daemon/listener to facilitate 
more external or public callbacks in order to improve [detection of SSRF](https://github.com/zaproxy/zaproxy/issues/3022) and other related vulnerabilities.

https://ssrfdetector.com/ was an online service for detecting Server Side Request Forgery (SSRF) vulnerabilities.
It was developed and maintained by Jake Reynolds and is open source https://github.com/jacobreynolds/ssrfdetector 
It may be used for inspiration/ideas as well as other projects such as sleepy-puppy (Netflix), etc. 

##### Expected Results

* Create or suggest a suitable alternative to SSRFDetector, and integrate it with ZAP in order to be able to detect SSRF vulnerabilities
* Code that conforms to our Development Rules and Guidelines

##### Getting Started

* Have a look at the ZAP [CONTRIBUTING](https://github.com/zaproxy/zaproxy/blob/develop/CONTRIBUTING.md) guideline, especially the 'Coding' section.
* We like to see students who have already contributed to ZAP, so try fixing one of the bugs flagged as [IdealFirstBug](https://github.com/zaproxy/zaproxy/labels/IdealFirstBug).

##### Mentors
* [Simon Bennetts](mailto:psiinon@gmail.com) and the ZAP core team.

#### Idea Three: Your Idea

ZAP is a great framework for building new and innovative security testing solutions. If you have an idea that is not on this list then don’t worry, you can still submit it, we have accepted original projects in previous years and have even paid a student to work on their idea when we did not get enough GSoC slots to accept all of the projects we wanted.

##### Expected Results

* A new feature that makes ZAP even better
* Code that conforms to our Development Rules and Guidelines

##### Getting Started

* Have a look at the ZAP [CONTRIBUTING](https://github.com/zaproxy/zaproxy/blob/develop/CONTRIBUTING.md) guideline, especially the 'Coding' section.
* We like to see students who have already contributed to ZAP, so try fixing one of the bugs flagged as [IdealFirstBug](https://github.com/zaproxy/zaproxy/labels/IdealFirstBug).

##### Mentors
* [Simon Bennetts](mailto:psiinon@gmail.com) and the ZAP core team.

### [OWASP Juice Shop](https://owasp-juice.shop)

OWASP Juice Shop is probably the most modern and sophisticated insecure web application! It can be used in security trainings, awareness demos, CTFs and as a guinea pig for security tools! Juice Shop encompasses vulnerabilities from the entire OWASP Top Ten along with many other security flaws found in real-world applications!

To receive early feedback please:
- put your proposal on Google Docs and submit it to the OWASP Organization on Google's GSoC page in "Draft Shared" mode. 
- Please pick "juice shop" as Proposal Tag to make them easier to find for us. Thank you!

#### Challenge Pack 2020

##### Brief Explanation:

Ideas for potential new hacking challenges are collected in [GitHub issues labeled "challenge"](https://github.com/bkimminich/juice-shop/issues?q=is%3Aissue+is%3Aopen+label%3Achallenge). This project could implement a whole bunch of challenges one by one and release them over the course of several small releases. This would allow the student to work in a professional Continuous Delivery kind of way while bringing benefit to the Juice Shop over the duration of the project. Especially the added functionality from [GSoC Feature Pack 2019](https://agrawalarpit14.github.io/GSoC/) is still mostly void of challenges and offers a lot of interesting attack surface in the whole order and payment process.

Coming up with good additional ideas for challenges in the proposal could make the difference between being selected or declined as a student for this project!

##### Expected Results:
* 10 or more new challenges for OWASP Juice Shop (including required functional enhancements to place the challenges)
* Each challenge comes with full functional unit and integration tests
* Each challenge is verified to be exploitable by corresponding end-to-end tests
* Hint and solution sections for each new challenge are added to the "Pwning OWASP Juice Shop" ebook
* Code follows existing styleguides and passes all existing quality gates regarding code smells, test coverage etc.

##### Getting started:
* Get familiar with the architecture and code base of the application's rich Javascript frontend and RESTful backend
* Get a feeling for the high code & test quality bar by inspecting the existing test suites and static code analysis results
* Get familiar with the CI/CD process based on Travis-CI and several associated 3rd party services

##### Knowledge Prerequisites:
* Javascript, Unit/Integration testing, experience with (or willingness to learn) Angular and NodeJS/Express, some security knowledge would be preferable.

##### Potential Mentors:
* [Bjoern Kimminich](mailto:bjoern.kimminich@owasp.org) - OWASP Juice Shop Project Leader

#### Your idea

##### Brief Explanation:

You have an awesome idea to improve OWASP Juice Shop that is not on this list? Great, please submit it!

##### Getting started
* Get in touch with [Bjoern Kimminich](mailto:bjoern.kimminich@owasp.org) to discuss your idea

##### Expected Results:
* A new feature that makes OWASP Juice Shop even better
* Code follows existing styleguides and passes all existing quality gates regarding code smells, test coverage etc.

##### Knowledge Prerequisites:
* Javascript, Unit/Integration testing, experience with (or willingness to learn) Angular and NodeJS/Express, some security knowledge would be preferable.

##### Mentors:
* [Bjoern Kimminich](mailto:bjoern.kimminich@owasp.org) - OWASP Juice Shop Project Leader
