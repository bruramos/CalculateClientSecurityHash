# Calculate Client Security Hash
RPA project designed as one of the tests of the UiPath Advanced Course.

Process that:

- Open the ACME System 1 Web Application (https://acme-test.uipath.com).
- Log in to System 1. Required input data: email and password.
- Access the Dashboard - the central location, where the user can pick a specific menu item.
- Access the Work Items listing to view all the available tasks to be performed (Output data: Work Items).
- For each activity of the WI5 type, perform the following steps:
  - Open the Details page of the selected activity to retrieve the Client Details.
  - Open the SHA1 Online webpage (http://www.sha1-online.com), and provide the following input: ClientID-ClientName-ClientCountry. Replace all the variables with the corresponding values. Use dashes between each item and the above.
  - Retrieve the Client Security Hash value from the webpage.
  - Go back to Work Item Details and open Update Work Item.
  - Set the status to “Completed”. Add a comment with the obtained Security Hash.
- Continue with the next WI5 Activity.

Obs.: This process uses the REFramework inside the UiPath.

For more information regarding the process needs, see the document "Calculate Client Security Hash - Process Design Document.pdf"
