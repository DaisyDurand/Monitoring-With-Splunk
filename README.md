# Monitoring-With-Splunk
## Description
This project, powered by Splunk, strengthens security at "Vandalay Industries" by analyzing data for threats. Custom reports empower stakeholders to enhance defenses, while automated alerts enable swift response to suspicious activities, ensuring data protection.
## Environment Used
* Splunk
## Creating a Report To Determine Impact
"Vandalay Industries" provided us with a file which containted the system speeds around the time of the attack. Our task required the creation of a report to determine the impact of the DDOS attack on upload and download speed.

First we need to create a field to calculate the ratio of the upload speed to the download speed. To do this we use this command:
