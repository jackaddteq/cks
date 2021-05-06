# cks
```
root@controlplane:~/Assessor-CLI# ./Assessor-CLI.sh -i

--------------------------------------------------------------------------------------
   ,o88888o.    8888    d888888o.          ,o88888o.           8.    8888888888888888 
  8888    `88.  8888  .`8888:' `88.       8888    `88.        .88.         8888       
,88888      `8. 8888  8.`8888.   Y8     ,88888      `8.      .8888.        8888       
888888          8888  `8.`8888.         888888              .`88888.       8888       
888888          8888   `8.`8888.   888  888888             .8.`88888.      8888       
888888          8888    `8.`8888.  888  888888            .8`8.`88888.     8888       
888888          8888     `8.`8888.      888888           .8' `8.`88888.    8888       
`88888      .8' 8888 8b   `8.`8888.     `88888      .8' .8'   `8.`88888.   8888       
  8888    ,88'  8888 `8b.  ;8.`8888       8888    ,88' .888888888.`88888.  8888       
   `888888P'    8888  `Y8888P ,88P'        `888888P'  .8'       `8.`88888. 8888       
--------------------------------------------------------------------------------------
         Welcome to CIS-CAT Pro Assessor; built on 01/28/2021 02:03 AM
--------------------------------------------------------------------------------------
  This is the Center for Internet Security Configuration Assessment Tool, v4.3.1
          At any time during the selection process, enter 'q!' to exit.
--------------------------------------------------------------------------------------

Verifying application

Attempting to load the default sessions.properties, bundled with the application.
Started Assessment 1/1

Loading Benchmarks/Data-Stream Collections

Available Benchmarks/Data-Stream Collections:
 1. CIS Controls Assessment Module - Implementation Group 1 for Windows 10 v1.0.3
 2. CIS Controls Assessment Module - Implementation Group 1 for Windows Server v1.0.0
 3. CIS Google Chrome Benchmark v2.0.0
 4. CIS Microsoft Windows 10 Enterprise Release 2004 Benchmark v1.9.1
 5. CIS Ubuntu Linux 18.04 LTS Benchmark v2.0.1
 > Select Content # (max 5): 5

Selected 'CIS Ubuntu Linux 18.04 LTS Benchmark'

Assessment File CIS_Ubuntu_Linux_18.04_LTS_Benchmark_v2.0.1-xccdf.xml has a valid Signature.
Assessment File CIS_Ubuntu_Linux_18.04_LTS_Benchmark_v2.0.1-xccdf.xml has a valid Signature.
Profiles:
1. Level 1 - Server
2. Level 2 - Server
3. Level 1 - Workstation
4. Level 2 - Workstation
 > Select Profile # (max 4): 1

Selected Profile 'Level 1 - Server'

Obtaining session connection --> Local
Connection established.  
Selected Checklist 'CIS Ubuntu Linux 18.04 LTS Benchmark'
Selected Profile 'Level 1 - Server'
Starting Assessment
----------------------- ASSESSMENT TARGET -----------------------------------
       Hostname: controlplane
        OS Name: linux
     OS Version: 5.4.0-1042-gcp
OS Architecture: x86_64

Interfaces:
  Name: lo
    IP: 127.0.0.1
   MAC: 00:00:00:00:00:00
  Name: docker0
    IP: 172.12.0.1
   MAC: 02:42:3e:66:78:c9
  Name: flannel.1
    IP: 10.244.0.0
   MAC: 02:f8:ed:75:83:8d
  Name: cni0
    IP: 10.244.0.1
   MAC: 3a:bc:da:72:c4:2a
  Name: eth0@if14683
    IP: 10.14.15.3
   MAC: 02:42:0a:0e:0f:03
  Name: eth1@if14685
    IP: 172.17.0.15
   MAC: 02:42:ac:11:00:0f
-----------------------------------------------------------------------------

Starting Assessment - Date & Time: 05-06-2021 14:54:08
-----------------------------------------------------------------------------
 Checklist Title: CIS Ubuntu Linux 18.04 LTS Benchmark
    Checklist ID: xccdf_org.cisecurity.benchmarks_benchmark_2.0.1_CIS_Ubuntu_Linux_18.04_LTS_Benchmark
   Profile Title: Level 1 - Server
      Profile ID: xccdf_org.cisecurity.benchmarks_profile_Level_1_-_Server

Assessing Platform Applicability
- Resolving Values.................................................................................. <1 second: Done
- Collecting 3 System Characteristics
- Evaluating Definitions


- Will collect 36 SCE Components

Starting assessment of OVAL Definitions:
- Resolving Values.................................................................................. 


229/241: Ensure users' home directories permissions are 750 or more restrictive..................... Fail
230/241: Ensure users own their home directories.................................................... Pass
231/241: Ensure users' dot files are not group or world writable.................................... Pass
232/241: Ensure no users have .forward files........................................................ Pass
233/241: Ensure no users have .netrc files.......................................................... Pass
234/241: Ensure users' .netrc Files are not group or world accessible............................... Pass
235/241: Ensure no users have .rhosts files......................................................... Pass
236/241: Ensure all groups in /etc/passwd exist in /etc/group....................................... Pass
237/241: Ensure no duplicate UIDs exist............................................................. Pass
238/241: Ensure no duplicate GIDs exist............................................................. Pass
239/241: Ensure no duplicate user names exist....................................................... Pass
240/241: Ensure no duplicate group names exist...................................................... Pass
241/241: Ensure shadow group is empty............................................................... Pass

-----------------------------------------------------------------------------
 ***** Assessment Results Summary *****
-----------------------------------------------------------------------------
   Total # of Results: 241
 Total Scored Results: 180
           Total Pass: 103
           Total Fail: 76
          Total Error: 1
        Total Unknown: 0
 Total Not Applicable: 0
    Total Not Checked: 20
   Total Not Selected: 37
  Total Informational: 4
-----------------------------------------------------------------------------
 ***** Assessment Scoring *****
-----------------------------------------------------------------------------
         Score Earned: 103.0
    Maximum Available: 180.0
                Total: 57.22%
-----------------------------------------------------------------------------

- Generating Checklist Results...

Ending Assessment - Date & Time: 05-06-2021 15:00:07
Total Assessment Time: 6 minutes
- Generating Asset Reporting Format.
- Collecting Checklist Results.
- Combining Results.
- Saving Results.
- Generating Data-Stream Collection.
- Data-Stream Collection Generated.
- Asset Reporting Format Generated.

 ***** Writing Assessment Results ***** 
 - Reports saving to /root/Assessor-CLI/reports
 -- controlplane-CIS_Ubuntu_Linux_18.04_LTS_Benchmark-20210506T150007Z.html
Assessment Complete for Checklist: CIS Ubuntu Linux 18.04 LTS Benchmark
-----------------------------------------------------------
Disconnecting Session.
Finished Assessment 1/1
Exiting; Exit Code: 0
```
