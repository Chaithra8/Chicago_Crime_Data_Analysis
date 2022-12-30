# "Chicago_Crime_Data_Analysis" 

This dataset reflects reported incidents of crime (with the exception of murders where data exists for each victim) that occurred in the City of Chicago from 2001 to present. Using this CSV file we're solving few problem statments using spark scala & visualizing them through graph & table view.

Data source - https://data.cityofchicago.org/Public-Safety/Crimes-2001-to-Present/ijzp-q8t2
Data Column Description 
1.	ID- Unique identifier of the record
2.	Case No – Chicago police department RD number (Record Division Number), which is unique to the incident.
3.	Date – Date when the incident occurred.
4.	Block – The partially redacted address where the incident occurred, placing it on the same block as the actual address.
5.	IUCR- Illinois Uniform Crime Reporting is directly linked to primary type and description.
6.	Primary Type- Primary description of IUCR.
7.	Description – Secondary Description of the IUCR code, sub-category of primary description.
8.	Location Description- Description of the location where the incident occurred.
9.	Arrest- Indicates whether an arrest was made.
10.	Domestic- Indicates whether the incident was domestic related as defined by Illinois Domestic Violence Act.
11.	Beat- Indicates the beat where the incident occurred. Beat is a smallest police geographic area – each beat as dedicated police beat car. 3-5 beats make up a police sector, and three sectors make up a police district. The Chicago police department has 22 police districts.
12.	District - Indicates the police district where the incident occurred
13.	Ward- The ward (City Council district) where the incident occurred.
14.	Community area - Indicates the community area where the incident occurred. Chicago has 77 community areas.
15.	FBI Code- Indicates the crime classification as outlined in the FBI's National Incident-Based Reporting System (NIBRS). 
16.	X Coordinate - The x coordinate of the location where the incident occurred in State Plane Illinois East NAD 1983 projection. This location is shifted from the actual location for partial redaction but falls on the same block.
17.	Y Coordinate - The y coordinate of the location where the incident occurred in State Plane Illinois East NAD 1983 projection. This location is shifted from the actual location for partial redaction but falls on the same block.
18.	Year - Year the incident occurred.
19.	Updated On - Date and time the record was last updated.
20.	Latitude- The latitude of the location where the incident occurred. This location is shifted from the actual location for partial redaction but falls on the same block.
21.	Longitude - The longitude of the location where the incident occurred. This location is shifted from the actual location for partial redaction but falls on the same block.
22.	Location - The location where the incident occurred in a format that allows for creation of maps and other geographic operations on this data portal. This location is shifted from the actual location for partial redaction but falls on the same block.

Below are the obtained output foreach problem statment
## Problem Statements:
   1.  How the number of various crimes changed over time in Chicago?
   
       <img src="https://github.com/Chaithra8/Chicago_Crime_Data_Analysis/blob/main/Output_image/PS1.png" width=50% height=50%>
       
       Conclusion: As we can see in the line graph, the lines corresponding to most of the crimes particularly that of the major crimes are falling down although there are some fluctuations. We can say over the past 20 years most of the crimes have decreased in numbers. At the same time we are seeing for some major crimes like theft, weapons violation etc. the rates are pretty high still and that's a major issue of concern.
       
   2. How have the number arrests corresponding to the crimes changed over time in Chicago?
    
       <img src="https://github.com/Chaithra8/Chicago_Crime_Data_Analysis/blob/main/Output_image/PS2.png" width=50% height=50%>
       
       Conclusion: From the Graph we can conclude that the number of arrests has gradually decreased If we consider the time frame from 2001 to 2020.
       
   3. Which contiguous months show largest variation in crime?
    
       <img src="https://github.com/Chaithra8/Chicago_Crime_Data_Analysis/blob/main/Output_image/PS3.png" width=50% height=50%>
       
       Conclusion: By using the above approach, we found that March is the month with largest variation that can be visualized with the query as well as bar graph.
      
   4. Which quarter was the most peaceful compared to the previous quarter?
        
       <img src="https://github.com/Chaithra8/Chicago_Crime_Data_Analysis/blob/main/Output_image/PS4.png" width=50% height=50%>
       
       Conclusion: By using the above approach, we found that third quarter is peaceful compared to previous quarter and can be visualized with the query as well as bar graph.
       
   5. Are there any trends in the crimes being committed?
    
       <img src="https://github.com/Chaithra8/Chicago_Crime_Data_Analysis/blob/main/Output_image/PS4.png" width=50% height=50%>
       
       Conclusion: By using the above approach, we found that 2018 is the year with minimum change in the crime trend and 2020 is the year with maximum change in the crime trend. We are visualizing the change in the trend using line graph.
       
   6. In which locations crimes are being committed frequently?
    
       <img src="https://github.com/Chaithra8/Chicago_Crime_Data_Analysis/blob/main/Output_image/PS6.png" width=50% height=50%>
       
       Conclusion: From the above graph, we can conclude that Street is the location where crimes are being committed frequently.
       
   7. Are there certain high crime locations for certain crime?
    
       <img src="https://github.com/Chaithra8/Chicago_Crime_Data_Analysis/blob/main/Output_image/PS7.png" width=50% height=50%>
       
       Conclusion: By referring to the table and bar graph, we can easily say, what are locations that are more prone to a particular type of crime. For example, we are seeing street is the place where theft happens the most.
       
   8. In which locations the frequent crimes are being committed?
    
       <img src="https://github.com/Chaithra8/Chicago_Crime_Data_Analysis/blob/main/Output_image/PS8.png" width=50% height=50%>
       
       Conclusion: From the above graph we can conclude that the five frequent crimes are being committed in Street maximum number of times.
     
       
