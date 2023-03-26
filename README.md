# Automate-Data-Import-and-Arrangement-from-API-using-Google-Apps-Script


This Google Apps Script automates the process of importing data from an API and arranging it in a Google Sheet.

Setup
Create a new Google Sheet.
Open the script editor by clicking on Tools > Script editor.
Copy and paste the code from the code.gs file into the script editor.
Replace the API URL in the importDataFromAPI function with your API endpoint.
Save the script.
Create a new trigger by clicking on Edit > Current project's triggers, then click on Add Trigger.
Select dailyUpdate as the function to run.
Set the Events field to Time-driven.
Set the Time based field to Day timer, and select the time of day you want the script to run.
Click Save.
How it works
The script has three functions:

importDataFromAPI: This function fetches data from an API and adds it to a sheet named Sheet1.
getMostSearchedKeywords: This function calculates the search volume of each keyword in the Sheet1 and adds the results to a new sheet named Keyword Frequencies.
dailyUpdate: This function runs the importDataFromAPI and getMostSearchedKeywords functions daily at the time specified in the trigger.
The importDataFromAPI function fetches data from an API and adds it to Sheet1. The API endpoint can be replaced with the URL of any API that returns JSON data.

The getMostSearchedKeywords function calculates the search volume of each keyword in Sheet1 and adds the results to a new sheet named Keyword Frequencies. This sheet is created if it does not already exist.

The dailyUpdate function runs the importDataFromAPI and getMostSearchedKeywords functions daily at the time specified in the trigger. This ensures that the data in the sheets is always up to date.

Conclusion
This Google Apps Script automates the process of importing data from an API and arranging it in a Google Sheet. It runs daily at the time specified in the trigger, ensuring that the data in the sheet is always up to date.