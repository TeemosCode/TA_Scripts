# Automation of sending emails to students from spreadsheet data

Run the ```automate_email_sending_CS41l.py``` locally once everything is set up.

Actions of each email sent by the program would be printed on the standard output for users' own confirmation.

The code was developed to be as flexible for a user in the future as possible.
As of now, students' spreadsheet would need to be converted into csv to work with this script. (Can be changed to other formats in the code by the user).

important information of a TA should be put into the global variables of:
```
MY_EMAIL_PROVIDER = "smtp.outlook.com"
# Change the following global variables based on your own information
# The first one is just as an example
STUDENT_INFO_FILE = "cs411_Student_info_test.csv"  # This is used as a CSV file. The following logic handles it as a CSV.
MY_OWN_EMAIL_ADDRESS = "[something]@illinois.edu"
EMAIL_PASSWORD = "[password]"  # Best to put this else where and read it in
EMAIL_SUBJECT = "Spring 2020 CS411 Project Track 1 - Assemble!"
MY_NAME = "Roger Ho"
MY_UIN = ""
```

Actions for a user to process their spreadsheet or whatever data schema they are holding for student's information should be added or changed to the method ```process_user_automation_code``` under the ```EmailAction``` class.



If the user finds the classes and modularized code annoying to read and follow. Feel free to just use the easy version ```automate_boring_email_send_action_to_bunch_of_newibies.py```
