# Monitoring-With-Splunk
## Description
This project, powered by Splunk, strengthens security at Company A by analyzing data for threats. Custom reports empower stakeholders to enhance defenses, while automated alerts enable swift response to suspicious activities, ensuring data protection.
## Environment Used
* Splunk

## Task 1
Uploaded a file which containted the system speeds around the time of the attack. Our task required the creation of a report to determine the impact of the DDOS attack on upload and download speed.

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

## Task 2

 Using Nessus vulnerability scanners, we pulled the last 24 hours of scans to search for critical vulnerabilites. This task involved creating a report determining how man crtical vulnerabilites exist on the customer data server. After, we created an alert fo notify the team if critical vulnerabilites reappears on this server.

 ### To create a report that shows the the count of critical vulnerabilites from the customer database server:

 To filter this information for the report we use this command:

![Nessus scan command results ](https://github.com/DaisyDurand/Monitoring-With-Splunk/assets/147094227/715dc8ac-b977-4be5-bfdc-c97a8d425f81)

This is the saved report:

![Nessus Report](https://github.com/DaisyDurand/Monitoring-With-Splunk/assets/147094227/b784abd3-7ff8-447d-8b38-a1d1b7e32b78)

### Creating an Alert

![Alert config 1](https://github.com/DaisyDurand/Monitoring-With-Splunk/assets/147094227/fe6b94c6-1bac-4b07-9746-3684e801655a)

![Alert config 2](https://github.com/DaisyDurand/Monitoring-With-Splunk/assets/147094227/bb518ca2-9fee-4cb0-86b6-173b0de33f1d)

![Alert config 3](https://github.com/DaisyDurand/Monitoring-With-Splunk/assets/147094227/e3eeebae-8743-443d-8ea5-6e2eba8c124f)

![Alert config 4](https://github.com/DaisyDurand/Monitoring-With-Splunk/assets/147094227/510dbd97-93a1-4522-a616-82dd087642e0)

![Alert config 5](https://github.com/DaisyDurand/Monitoring-With-Splunk/assets/147094227/21160a0e-db92-4269-977c-d3b1334d8c50)

![Alert config 6](https://github.com/DaisyDurand/Monitoring-With-Splunk/assets/147094227/6c91be87-f192-47c6-abd3-5329bb686320)

![Alert has been saved](https://github.com/DaisyDurand/Monitoring-With-Splunk/assets/147094227/300cb629-49aa-472d-a29f-480d427a7b15)

![Alert completion](https://github.com/DaisyDurand/Monitoring-With-Splunk/assets/147094227/6545a8c2-6f8e-40d1-a81a-e20397fbc503)

## Findings

There are 98 critical vulnerabilities from the customer database server.

## Task 3

A server has been experiencing a brute force attacks into the administrator account. 

### Comand to filter the information:

![Results for brute attack](https://github.com/DaisyDurand/Monitoring-With-Splunk/assets/147094227/dcbd7cb1-2005-4892-a21a-0f8e4f5df7d6)

### Creating the alert:

![Alert for thresh config](https://github.com/DaisyDurand/Monitoring-With-Splunk/assets/147094227/c6419bc8-1d39-4b08-947b-f47c7614c0e1)

![Alert for thresh config 1](https://github.com/DaisyDurand/Monitoring-With-Splunk/assets/147094227/146e391b-0298-40d3-a22c-8e45410d7310)

![Alert for thresh config 2](https://github.com/DaisyDurand/Monitoring-With-Splunk/assets/147094227/a28ca17b-b0ab-42ed-9730-e65cd4800128)

![Alert for thresh config 3](https://github.com/DaisyDurand/Monitoring-With-Splunk/assets/147094227/26157bff-763d-4d8c-aaed-971ee9edbbfa)

![Alert saved for brute](https://github.com/DaisyDurand/Monitoring-With-Splunk/assets/147094227/06426d7a-df8b-41d9-945c-6486211686c0)

![Brute force alert completion](https://github.com/DaisyDurand/Monitoring-With-Splunk/assets/147094227/4a7cd3d4-71a4-4d81-9fc4-5f2d189faf41)
 
## Findings

The brute forced attack occurred on February 21st 2020 at 4 AM. The baseline for normal activity is 200 and the threshold is 230.
