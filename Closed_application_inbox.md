
### 1.2.4	Closed Application

#### 1.2.4.1	Process Flow

**Step 1.** In the backend, At the end of the day, LAPS updates the closed status in the PMV tables for accounts that are closed in CBS.

**Step 2.**	The system runs a scheduler to find loan accounts that have the closed status updated in PMV tables.

**Step 3.**	The system calls the Close API to update the closure status for all identified accounts in the portal.

**Step 4.**	If close status is successful, accounts successfully updated in the portal appear in the **Closed in Portal** tab and accounts remain visible for 30 days from the closure date.

**Step 5.**	If close status is failed, accounts failed to update appear in the **Update Failed** tab and accounts remain visible for 30 days.

**Step 6.**	Navigate to the **Closed loan inbox** and click **Update failed tab**.

**Step 7.**	Click **Update status** for each application. System triggers the Call Close API.

**Step 8.**	If successful, the system disables the button for that account.

**Step 9.**	Clicks **Update Status for All** to update all pending accounts displayed on the screen.

**Step 10.** The system triggers the **Call Close API** for all accounts with pending closure status.

**Step 11.** After the update, the system displays an alert showing the count of successfully updated accounts.

#### 1.2.4.2	Closed Application Inbox

**Step 1.** Click Closed Application Inbox the set of tabs will display as shown below

![Closed Application Inbox](Closed application inbox.png)

**Step 2.** In the **Closed in Portal inbox**, Loan accounts for which the status update to the portal is successful at the time of running scheduler will be displayed.

**Step 3.** Click **Download Report** to download the date and displayed in excel format.

![Closed Application](Closed application.png)

**Step 4.** Loan accounts for which the status update to the portal failed at the time of running scheduler will be displayed in **Update Failed**.

**Step 5.** Click **Update status** to manually update the closure status, if the update is successful, system will display “Update successful” message.

![Update Application](Update application.png)

**Step 6.** If any technical error occurs, system will display error to the user.

**Step 7.**	Click **Update all** , system will trigger the status update API for all the applications that are displayed on screen.

![Update all button](Update all button.png)

## 1.3	Summary

In this chapter, you learned how to process loan applications in PSB PM Vishwakarma Yojana portal, including auto-sanctioned and branch-assisted flows, from pulling applications and running validations to account handoff, disbursement, and updating statuses to the PMV portal.

Click here to view [Closed Application](PSB-PMV-scheme-user-manual
/Closed_application_inbox.md)

Click here to view [Branch Assisted Journey](PSB-PMV-scheme-user-manual
/Branch_assisted_journey.md)

Click here to view [Sanction Inbox](#SanctionedApplications)
