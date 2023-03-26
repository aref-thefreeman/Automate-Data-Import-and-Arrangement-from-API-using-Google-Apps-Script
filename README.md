# Google Apps Script for Importing and Arranging Data from an API

This Google Apps Script automates the process of importing data from an API and arranging it in a Google Sheet.

## Overview

This script performs two main tasks:

1. Imports data from an API endpoint and stores it in a Google Sheet.
2. Sorts the imported data by keyword frequency and displays it in a separate sheet.

## Prerequisites

Before using this script, you'll need to:

- Have a Google account and access to Google Sheets.
- Obtain an API endpoint URL that returns JSON data.

## Setup

To set up this script, follow these steps:

1. Create a new Google Sheet.
2. Open the Script Editor by selecting `Tools` -> `Script editor` from the menu.
3. Copy and paste the script code into the Script Editor.
4. Replace the `API_ENDPOINT_URL` variable with your API endpoint URL.
5. Save the script and give it a name.
6. Run the `dailyUpdate` function to import and arrange the data.

## File Structure

The main script file is `code.gs`, which contains the following functions:

- `importDataFromAPI()`: Imports data from an API endpoint and stores it in the active sheet.
- `getMostSearchedKeywords()`: Sorts the imported data by keyword frequency and displays it in a new sheet.
- `dailyUpdate()`: Runs `importDataFromAPI()` and `getMostSearchedKeywords()` to update the data daily.

## Usage

To use this script, you'll need to:

1. Set up the script by following the steps in the Setup section.
2. Run the `dailyUpdate()` function manually or schedule it to run automatically.

## Schedule the Script

To schedule the script to run automatically:

1. Open the Script Editor.
2. Click `Edit` -> `Current project's triggers`.
3. Click the `+ Add Trigger` button.
4. Set the trigger to run `dailyUpdate` function every day at a specific time.
5. Click `Save`.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
