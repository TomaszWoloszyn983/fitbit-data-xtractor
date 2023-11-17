# fitbit-data-xtractor
A Bot created to extract data and statistics from Fitbit website.

The  application uses Robotic Process Automation to extract data and statistics from Fitbit website and write retrieved data into an excel file.



![AmIResponsive](documentation/images/fitbit_dashboard.png)


## Features


- Extracts data such as Calories consumed and burned, nutritions, activites and sleep, from the Fitbit.com website.
- Write data to Excel files
- Synchronize all the extracted data and write them into one final excel table.

#### Flowchart Processes

![AmIResponsive](documentation/images/flowchart.png)

- Start application. 
Opens the Chrome Browser on the fitbit.com website
- Flow Decision 
if the website is succesfully opened it directs the workflow to get data processes.
If the website is not succesfully opened it directs the flowchart to closing browser process.
- Invoke Workflow ReadWeightData.
Extract data from the Weight page, such as Date, Weight and Body Fat.
Assigns this values into a temporary excel file.
- Invoke Workflow GetActivityData
Extract data from the Activity page, such as Calories Burned, Nunber of Steps, Floors and Distance.
Assigns this values into a temporary excel file.
- Invoke Workflow GetCaloriesAndNutritions
Extract data from the Food page, such as Calories consumed, Fat, Fiber, Carbohydrates, Sodium, Proteins and Water.
Assigns this values into a temporary excel file.
- Invoke Workflow GetSleepData
Extract data from the Sleep page, such as sleep start time, sleep end time and sleep duration.
Assigns this values into a temporary excel file.
- Close All Applications.
- Merge Tables
Proces all data from temporary files and generate the final ouput file.

### Page

![BackgroundImage](documentation/images/fitbit_activityPage.png)



### Future Features

- Credentials
- Add Read Activities Details process


## Tools & Technologies Used

- UiPath
- Microsoft Excel


## Database Design

No data base is used at this stage of the application. It is considering to use some kind of data storage for small pieces of informations, such as players result to be stored in the browsers storage.


## Deployment


## Local Deployment
In order to make a local copy of this project, you can clone it. In your IDE Terminal, type the following command to clone my repository:

git clone https://github.com/TomaszWoloszyn983/fitbit-data-xtractor

## Credits


### Acknowledgements
