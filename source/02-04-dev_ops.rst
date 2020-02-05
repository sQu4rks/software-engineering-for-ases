DevOps and Deployment
=====================

Software Deployment is the process of making a piece of software available to users. 

Before the internet, deployments were expensive, infrequent and bulky affairs but 
due to the ability to deliver new versions over the internet software 
development, especially within web applications, has become a near continuous process.

At its core software deployment is not about deploying software but about managing 
risk. Businesses need to change in order to improve their product. However every 
change that is applied to a working system has the potential to break it. Thus we 
need techniques and processes that allow us to mitigate risk while still rapidly 
deploying new changes. 

**Continuous Integration** or CI is the process of continuously integrating new changes/components 
of the source code into the application. Instead of having one big "push day" where changes are 
merged we continuously add changes as they are made available by the development team.

Continuous Integration Pipelines usually start with a Source Code Management (SCM) change. 
New code has been pushed by a developer. What happens next depends on the organization but some 
common steps are

* Clone the code
* Compile the code (if needed)
* Test the code - This can include running unit, integration and static tests as well as testing for code coverage(what percentage of source code is actually tested by test cases) or memory leak tests.
* Report - Either via a dashboard, e-mail, chat or other means of communication
* (Deploy) - Code *could* be automatically deployed into production or staging environments

C'mon tell me about DevOps
--------------------------

DevOps, short for Development Operations, is a set of practices that aims to combine 
software development with infrastructure operations required to run the changes. It aims
at providing a shorter software development life cycle while providing continuous delivery
with high software quality. 

Before DevOps organizations often had a noticeable difference between the software engineers
writing code and the infrastructure engineers maintaining the infrastructure the code 
would ultimately run on. 

As a cross-functional approach DevOps uses different tool chains to deliver software. 

1. Coding - Code development, especially Source Code Management and Version Control Software
2. Building - Continuous Integration tools (like Jenkins, CircleCI or TravisCI)
3. Testing - Continuous testing based on existing test cases
4. Packaging - artifact repositories providing access to static components
5. Releasing - change management and Release automation 
6. Configuration - Infrastructure-as-Code 
7. Monitoring - Application performance monitoring and error monitoring

Continuous delivery (CD) and DevOps are closely related. CD focuses on the process of 
automating the process of software delivery while DevOps additionally focuses on the 
collaboration aspects within a organization.
