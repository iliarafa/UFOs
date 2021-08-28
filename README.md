# UFOs

### Project Purpose 
This project aims to create a webpage featuring a dynamic table to provide an in-depth analysis of UFO sightings by allowing users to filter for multiple criteria at the same time. 

### Results
This webpage features a very simple and user friendly interface to specify the given search criteria. Five filters are in place. By default the table is populated with our initial set of data. The process is as follows : 

#### _narrowing down the search: 
**Step 1**: Enter value in desired field. \
**Step 2**: Hit return OR move to the next field. Both actions display the updated filtered table. \
**Step 3**: Enter value in next field and repeat the process in Step 2. 


#### _broadening the search: 
**Step 1**: Backspace on the field you want to remove until you reach the placeholder value. \
**Step 2**: Hit Return, click on any point of the page's body, or move to the next field. 

### Summary 

Due to our data file's initial structure we faced a serious drawback that could affect the functionality of the page. The date format was not correctly specified. Our filter initially accepted the following date format : M/DD/YYYY. That works fine for the data we have now as all sightings happened in January. If we later have a sighting in October and we perform a search based on the date filter we will get an empty table. To resolve this we would have to alter the value for the Date key to the following format : MM/DD/YYYY

In the same way State and City names are in lower case letters which might confuse a user expecting uppercase letter for state values and capitalized city names as is the common practice. If for example one enters CA for California will get no results.

Here is our initial data displayed on the table :
![](images/before.png)

This could be resolved by defining "example" placeholders like "st" for State or "city" for City but correcting our data file is surely a more efficient process. 

Here is what the corrected data looks like now : 


In terms of readability, the duration format has to be in the same unit. Either seconds or minutes so it is easily comparable. We also have to use either minutes or mins. or min but all these at the same time. This also goes back to modifying our data.js

