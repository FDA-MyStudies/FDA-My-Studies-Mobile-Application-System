# FDA MyStudies Mobile Application System

### Background

The FDA MyStudies App is designed to facilitate direct patient input of real world data which can be linked to electronic health data,
thereby supporting traditional clinical trials, pragmatic trials, observational studies, and registries. It was developed by the FDA and
private sector partners, but source code and documentation have been released to the public as open source software so the app and data
storage system can be reconfigured and rebranded by other organizations conducting clinical research. It can also be improved by software
developers.

The system has several important features. The data storage environment is secure and supports controls necessary for compliance with
21 CFR Part 11 and the Federal Information Security Management Act, so it can be used for trials under Investigational New Drug oversight.
The app is configurable to accommodate different therapeutic areas, health outcomes, surveys, and consents, which reduces or eliminates
software development hurdles for those who wish to deploy it. The data storage environment is scalable and partitioned to support multiple
clinical trials from different organizations, large multi-site trials, and “distributed database” studies.

These resources provide detailed background information about the FDA MyStudies system:

- [The FDA MyStudies App: A Patient Centered Outcomes Research Trust Fund Enabler for Distributed Clinical Trials And Real World Evidence Studies](https://www.fda.gov/media/119835/download)
- [FDA's MyStudies Application Technical Background](https://www.fda.gov/drugs/science-and-research-drugs/fdas-mystudies-application-app-technical-background)

### This Repository

This repository contains all the necessary code for running the FDA MyStudies mobile applications (iOS and Android), web 
configuration portal (WCP), and storage environment. The mobile apps and WCP were developed by Boston Technology Corporation. 
The registration server and storage environment are extensions of LabKey Server, a platform developed by LabKey and 
available under the Apache 2.0 license. All development occurred under the direction of FDA and the Harvard Pilgrim Research Institute (HPHCI).

This Git repository includes six submodules, one for each major component of the FDA MyStudies system. If you're not familiar with submodules,
you may want to review the [Git Submodules documentation](https://git-scm.com/book/en/v2/Git-Tools-Submodules). We strongly recommend upgrading
to the latest Git version to ensure you have full support for submodules. To clone this repository and automatically initialize and update each
submodule, use the `--recurse-submodules` flag, for example:

```
git clone --recurse-submodules https://github.com/FDA-MyStudies/FDA-My-Studies-Mobile-Application-System.git
```
Once the repository and submodules are cloned, you can periodically pull all the latest changes using:
```
git pull --recurse-submodules
```

This consolidated repository provides access to the latest code for every FDA MyStudies component. We are actively working on providing a
consolidated build process that can compile every submodule into a deployable component from this top-level repository. In the meantime,
those who wish to develop or build the MyStudies components will need to visit the individual repositories and follow the build instructions
to build each component separately.

### Documentation

Set up requires the deployment and configuration of the following components. Development of each component is done in one or more submodules;
links to the submodule version most recently published to production are provided here. 

- the **Registration Server** where participants sign up and create an account \(UserReg-WS\)
- the **Mobile Client App** into which participants enter data \(Android or iOS\)
- the **Response Server** which handles and stores the responses sent by the Mobile App \(Response\)
- the **Web Configuration Portal** where administrators design research questionnaires \(WCP and WCP-WS\) 

Setup Instructions:

- [FDA MyStudies: Technical Setup Document](https://www.labkey.org/FDAMyStudiesHelp/wiki-page.view?name=setupInstructions)

### Learn More

- [FDA MyStudies Documentation](https://www.labkey.org/FDAMyStudiesHelp/project-begin.view?)
- [Webinar: An Introduction to FDA MyStudies: An Open-Source, Digital Platform to Gather Real World Data for Clinical Trials and Research Studies – May 9, 2019](https://www.fda.gov/drugs/cder-small-business-industry-assistance-sbia/introduction-fda-mystudies-open-source-digital-platform-gather-real-world-data-clinical-trials-and)
