# Monitoring-With-Splunk
## Description
This project, powered by Splunk, strengthens security at "Company A" by analyzing data for threats. Custom reports empower stakeholders to enhance defenses, while automated alerts enable swift response to suspicious activities, ensuring data protection.
## Environment Used
* Splunk
## Creating a Report To Determine Impact
"Company A" provided us with a file which containted the system speeds around the time of the attack. Our task required the creation of a report to determine the impact of the DDOS attack on upload and download speed.

## Task 1

### First we need to create a field to calculate the ratio of the upload speed to the download speed. To do this we use this command:

![Creating_Ratio_Field](https://github.com/DaisyDurand/Monitoring-With-Splunk/assets/147094227/ecfde936-7e4b-4c6a-91d0-090fa6322ddc)

### These are the results:

![ratio_results 2](https://github.com/DaisyDurand/Monitoring-With-Splunk/assets/147094227/19d283d6-d942-4b6b-97af-b41de380b46c)

### Next to create a table: 

![Table command in splunk](https://github.com/DaisyDurand/Monitoring-With-Splunk/assets/147094227/83a74da5-bb14-476d-bb0e-03269ff44642)

### These are the results:

![Table columns 1](https://github.com/DaisyDurand/Monitoring-With-Splunk/assets/147094227/e997d53f-b317-4abd-b0fb-484afb267b51)

![Table columns 2](https://github.com/DaisyDurand/Monitoring-With-Splunk/assets/147094227/8a5f647f-89b4-42e9-9227-3d22d65dbf23)

![Table columns 3](https://github.com/DaisyDurand/Monitoring-With-Splunk/assets/147094227/ba40081f-f3a6-48cf-880a-9ac9ad181055)

### The following is a line chart displaying how the download_megabits and upload_megabits were affected during the attack:

![Approx_date_time_attack](https://github.com/DaisyDurand/Monitoring-With-Splunk/assets/147094227/922b267a-ebc9-45ce-803b-47e09b42b31e)

### The following images are reports:

![Report of table 1](https://github.com/DaisyDurand/Monitoring-With-Splunk/assets/147094227/3fd3056c-66a6-4f66-b16e-bca2ec96f49a)

![Line chart report](https://github.com/DaisyDurand/Monitoring-With-Splunk/assets/147094227/68e7d138-acbd-4951-938d-8bdb320c8bd5)

## Findings

Based on the reports the approximate date and time of the attck is February 22nd at 11:30 PM.
The systems were completely down at 2:30 PM on February 23rd. After 2:30 the systems started to come back up. A full recovery was made at 11:30 on the 23rd. It took approximately 9 hours for the systems to recover.

##Task 2

"Company A"
