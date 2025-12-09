
### 1.2.3	Branch Assisted Journey

#### 1.2.3.1	Process Flow

The application which failed in Pre BRE and Main BRE will display under branch assisted journey.

**Step 1.** The system enables the modify button for you to manually enter the operative account number to continue the journey.

**Step 2.**	The system initiates the BRE process.

**Step 3.**	The system retrieves customer details from CBS using the operative account number provided by the PMV Portal.

**Step 4.** The system handles CIBIL API initiation: 

    •	If initiation fails due to technical issues, the system updates the status to CIBIL API Failed and allows reinitiation.

    •	If initiation succeeds, the system waits for the response and then proceeds to BRE check.

**Step 5.**	The system runs the BRE check, upon BRE succeeds, the system updates the status to Approved, moves the application to the Auto Sanctioned Inbox, and triggers the Call Sanction API to update the PMV Portal.

**Step 6.**	After the application is sanctioned the flow of this application will be same as mentioned from [Step 4.](id="Loop") to step 12 as mentioned in sanctioned backend flow.

#### 1.2.3.2	Branch Assisted Inbox

**Step 1.** Click **Branch Assisted Inbox** the list of applications will display as shown below.

![Branch Assisted Journey](Branch assisted inbox.png)

**Step 2.** Click **View Application** to view the corresponding application.

![Details Tab](BA_View application.png)

**Step 3.** **Personal details**, **Communication details**, **loan details**, **business details** section are auto populated.

**Step 4.**	When the account number received from the PMS portal does not match any record in CBS, the CBS Customer Details section remains blank.

**Step 5.**	The system enables the **Modify** option, allowing the account number field to be edited. 

![Modify Account Number](Modify.png)

**Step 6.** Enter the correct savings account number in modify account number popup.

**Step 7.**	The system retrieves the corresponding CBS customer details and displays them in the CBS Customer Details section.

**Step 8.**	Once CBS details are available, the **Initiate Cibil & BRE** button becomes active.

**Step 9.**	Click **Initiate Cibil & BRE** to save the updated details and proceed to the next step.

**Step 10.** If CBS details are not available, the **Initiate Cibil & BR**E button remains disabled.

**Step 11.** Once the Cibil response is received, the system triggers the BRE check.

**Step 12.** If BRE fails, the system will mark the status as **Rejected** and status will be updated in PM Vishwakarma portal along with the rejection reason.

**Step 13.** On the successful completion of all the BRE parameters, the case will be marked as **Approved** digitally and the status will be reverse updated to the PM Vishwakarma portal.

> Note:
>Once the application is approved, system triggers the email to branches.

**Step 14.** Once the sanction is completed, application will be moved to Sanctioned inbox. You can initiate documentation from the Sanctioned Application section as mentioned in case of Auto sanctioned application. 

**Step 15.** The remaining flow will be same as auto sanctioned application.

**Step 16.** Reject button will be available to you till the application is sanctioned. Enter the reject reason in the remarks section. Once you reject the application the status will be updated to Portal with the rejection reason.

![Reject screen](Reject.png)

[Closed Application](https://github.com/Surya-Jaganathan/PSB-PMV-scheme-user-manual/blob/858615c2af6c8cc77ec117378a06e1eea910fd1b/Closed_application_inbox.md)

![Modify Account Number](Modify.png)

Click here to view [Branch Assisted Journey](PSB-PMV-scheme-user-manual
/Branch_assisted_journey.md)

Click here to view [Sanction Inbox](#SanctionedApplications)
