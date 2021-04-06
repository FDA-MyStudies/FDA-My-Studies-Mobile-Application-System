# FDA MyStudies Mobile Application System

The FDA MyStudies App is designed to facilitate direct patient input of real world data which can be linked to electronic health data,
thereby supporting traditional clinical trials, pragmatic trials, observational studies and registries. It was developed by the FDA and
private sector partners, but source code and documentation have been released to the public as open source software so the app and data
storage system can be reconfigured and rebranded by other organizations conducting clinical research and improved by software developers.
The FDA MyStudies App has several important features. The data storage environment is secure and supports controls necessary for compliance
with 21 CFR Part 11 and the Federal Information Security Management Act, so it can be used for trials under Investigational New Drug
oversight. The app is configurable for different therapeutic areas and health outcomes which reduces software development hurdles for
non-FDA users. The data storage environment is scalable and partitioned to support large multi-site trials or “distributed database” studies.

This repository contains all the necessary code for running the FDA MyStudies mobile applications (iOS and Android), web 
configuration portal (WCP), and storage environment. The mobile apps and WCP were developed by Boston Technology Corporation. 
The registration server and storage environment are extensions of LabKey Server, a platform developed by LabKey and 
available under the Apache 2.0 license. All development occurred under the direction of FDA and the Harvard Pilgrim Research Institute (HPHCI).

### Documentation

Set up requires the deployment and configuration of the following components. Development of each component is done in one or more submodules; links to the submodule version most recently published to production are provided here. 

- the **Registration Server** where participants sign up and create an account \(UserReg-WS\)
- the **Mobile Client App** into which participants enter data \(Android or iOS\)
- the **Response Server** which handles and stores the responses sent by the Mobile App \(Response\)
- the **Web Configuration Portal** where administrators design research questionnaires \(WCP and WCP-WS\) 

Setup Instructions:

- [FDA MyStudies: Technical Setup Document](https://www.labkey.org/FDAMyStudiesHelp/wiki-page.view?name=setupInstructions)

### Learn More

- [FDA MyStudies Documentation](https://www.labkey.org/FDAMyStudiesHelp/project-begin.view?)
- [FDA's MyStudies Application Technical Background](https://www.fda.gov/drugs/science-and-research-drugs/fdas-mystudies-application-app-technical-background)
