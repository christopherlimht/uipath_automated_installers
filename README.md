# UI path - automated installation of software
This is a test project of using UIpath to install software which installers do not have a automated unattended installation option. This test project is integrated with Servicenow and retrieves the list of software to be installed off ServiceNow using REST. Once all installation has been completed, serviceNow will be updated through Rest of the installation progress.

## Platforms used
1. UiPath 
2. ServiceNow - Orlando edition

## Pre-requisite
1. Creation of a business application and relevant tables on serviceNow
2. Modify HttpRequest block in unattended_installation workflow to reflect updated URL endpoint and data structure
3. Creation of a folder, "installers" in project root
4. Place the installers inside the newly created folder
5. Record the macro/Develop the RPA for each individual installer
6. Link all developed workflow up as per example in unattended_installation.xaml
7. Execute on unattended_installation.xaml through UIPath
