# Export Issues as CSV
## Background
This script was created to get around the export limits set in Jira. It exports data from a JQL filter as a CSV file and sends the file via email.

## Installation
### Scripts
1. Create a folder in the SIL Manager called Runner_Gadget
    * Create a file named **exportCSV.sil**
    * Copy the contents of the **exportCSV.sil** script from this repository into the script in your SIL Manager
2. Inside the Runner_Gadget folder create the following subfolders:
    * Data
        * Create a file named **csvMemes.csv**
        * Create a file named **customFields.csv**
        * Create a file named **defaultFields01.csv**
        * Create a file named **defaultFields02.csv**
        * Copy the contents of the scripts from this repository into the scripts in your SIL Manager
    * Param_Scripts
        * Create a file named **csv_params.sil**
        * Copy the contents of the **csv_params.sil** script from this repository into the script in your SIL Manager
2. Create a folder in the SIL Manager called Services
    * Create a file named **deleteZipFiles.sil**
    * Copy the contents of the **deleteZipFiles.sil** script from this repository into the script in your SIL Manager
### SIL Runner Gadget
1.  Go to a Jira Dashboard that is editable by the current user.
2.  Add the **Power Scripts SIL Runner Gadget** to the dashboard.
3.  Edit the widget
4.  Click the **+ Add** button on the widget
5.  Provide a _Name_ to the script. Example: "drawIO Execution"
6.  Select the **exportCSV.sil** file under _Exection script_
7.  Set the **Use custom parameters form?** option to **Yes**
8.  Select the **csv_params.sil** from the  file under _Exection script_
7.  Click the **Save** button
8.  Click the **Done** button

### Service
1. Go to SIL Scheduler in the Jira admin
2. Select **Add Job** from the upper right
3. Scheduler type

### Configuration

## Execution
