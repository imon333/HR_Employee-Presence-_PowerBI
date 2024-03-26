
# Employee Presence DATA



## Problem Statement

This dashboard helps the HR to understand better. It helps the HR know if their employee are present in the office or Home office or Sick leave or any half day. This Dashboard is only for 3 months but if any new months come , which can be easily used by the template .

Also they which month / day employee are woring more in the office or in the Home office.


### Steps followed 

- Step 1 : Load data into Power BI Desktop, dataset is a xlsx file.
- Step 2 : Open power query editor & in view tab under Data preview section, check "Colimn date ".
- Step 3 : As there are three different sheet with date column where our plan is to create one column with date for all data.
- Step 4 : It was observed that in none of the columns errors & empty values were present except column named "Arrival Delay".
- Step 5 : Also used to calclate total working day, holyday.
- Step 6 : Creating persent in perecntage also Home office and Sick leave.
- Step 7 : Then also visualize with a table with name of the employee also there are options to click for each months like April , May, June. 

    
- Step 8 : New measure was created to find perecntage of present in office.

Following DAX expression was written for the same,
        
        present % = DIVIDE([Present Days],'Measure Table'[Total Working Days],0)
        
A card visual was used to represent 'present in office'.

![A1 1](https://github.com/imon333/HR_Employee-Presence-_PowerBI/assets/140762800/a296aa60-700c-4261-90ff-9ce2e22bb189)

 - Step 9 :New measure was created to find perecntage of Home office.

Following DAX expression was written for the same,
        
        WFH % = DIVIDE([WFH Count],[Present Days],0) 
        
A card visual was used to represent 'Homw office'.
 
 
![A2](https://github.com/imon333/HR_Employee-Presence-_PowerBI/assets/140762800/5f26f90e-161a-40f4-ab8a-837db0f5bbae)

 
 - Step 10 : New measure was created to find perecntage of Sick leave.

Following DAX expression was written for the same,
        
        SL % = DIVIDE([SL Count],[Total Working Days],0) 
        
A card visual was used to represent 'Sick leave'.
 
 
 ![A3](https://github.com/imon333/HR_Employee-Presence-_PowerBI/assets/140762800/6ae65167-5a71-4131-89b8-4c4b5c315967)
 


# Snapshot of Dashboard (Power BI Service)

![POW DASH board](https://github.com/imon333/HR_Employee-Presence-_PowerBI/assets/140762800/b9633a93-a4e0-461e-9067-60a31a29eec6)


 
 # Report Snapshot (Power BI DESKTOP)

 
![Dashboard_upload](https://user-images.githubusercontent.com/102996550/174074051-4f08287a-0568-4fdf-8ac9-6762e0d8fa94.jpg)

