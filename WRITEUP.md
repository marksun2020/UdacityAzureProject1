# My choice between a VM or App Service

## Our application is:
- pure Web App, written on Python, has built-in support in App Service
- no special requirements for memory, cpu
- no special requirements for hardware

## App Service advantages 
- it takes more time and effords to prepare a VM, the App Service is ready for your software
- it takes more time and effords to load the software into VM, the App Service has a pipeline to load software automatically. We use Github + Github actions

## Neutral, difficult to compare
- both App Servcie and VM cann be scaled horisontally and vertically
- for the App Service we will pay for the application plan the whole time if the application is used or not. It depends on application plan and an VM configuration what is more expensive. For 60 minutes a day we can use test application plan for no cost

## Result
**App Service is a better choice for us**

## What would change the decision
- the application instance needs more than 14GB RAM or very intensive computation (more than 4 vCPUs necessary)
- dedicated hardware or software is necessary to be used
- support for a special programming language which is not supported by App Service
