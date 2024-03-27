Compiled March 2024.

# Overview

- [JIRA](#jira)
  - [Submitting a Ticket](#submitting-a-ticket)
  - [SC Board](#sc-board)
- [Archival Planner](#archival-planner)
  - [Blue Sheets and Merge Requests](#blue-sheets-and-merge-requests)
  - [Microsoft Flow](#microsoft-flow)
 
# JIRA
## Submitting a Ticket
 - Tickets are submitted through the [JIRA Help Center](https://unclibrary.atlassian.net/servicedesk/customer/portals) under the "Wilson Library Technical Services" portal. There are two sections of the portal to submit a request through: Archival Services (for finding aid or ArchivesSpace errors, processing requests, location remediation, or content warning creation/editing) and Bibliographic Services (for remediation of bioliographic records, location or size corrections in Sierra, content warning creation/editing, and metadata edits).
 - All Wilson Services tickets, including those from Tech Services staff, should be submitted through the portal. (There is a function to submit tickets through the back end of JIRA, but as of now we are not using this function).
## SC Board
 - Wilson tickets will appear in our Special Collections Technical Services board in JIRA. You can access the board [here](https://unclibrary.atlassian.net/jira/software/c/projects/SC/boards/65) or under Your work--boards--SC board after signing into your JIRA.
 - Once a ticket is submitted it will appear under the "backlog" column of our SC board under either the "Archival" or "Bibliographical" swim lane.
   - New archival tickets automatically tag and email Laura Smith, Dawne Lucas, and Jackie Dean.
   - New bibio tickets automatically tag and email all biblio people.
### Board Workflow 
  - When a ticket comes into the "backlog" column, any of the tagged users can move it into the "queued" column (for tickets awaiting work) or "in progress" column (for tickets being worked on). This can be done by dragging and dropping the ticket into the desired column in the board.
  - JIRA will prompt you to make a comment whenever changing columns. You can comment, either internally or to the submitter, or leave the box blank and continue.
#### Pending Response
If you are waiting for a response from the submitter before continuing work on a ticket, you can mark the ticket as "pending response" when under the "in progress" column by clicking on the "in progress" dropdown at the top right of the ticket and selecting "pending response from reporter."
![JIRA 6](https://github.com/llsmith305/images/blob/main/Jira_capture_6.png)

## Assigning a Ticket
Each ticket allows for one, and only one, assignee. You can assign a ticket to yourself or anyone else in TS by opening the ticket and navigating to the "assignee" field on the right side of the ticket. You can either click "assign to me" to assign to yourself, or search for an assignee by name. An email alert will be sent to the assignee.
![JIRA 1](https://github.com/llsmith305/images/blob/main/Jira_capture_1.png)
## Communication in a Ticket
After you open a ticket, you can scroll down to view the activity on that ticket, including all comments. You can add internal notes to TS people working on the ticket or comment out to the submitter of the ticket. You can @mention anyone within TS (or any watchers - see below) within these comments.
![JIRA 2](https://github.com/llsmith305/images/blob/main/Jira_capture_2.png)
### Watchers and Participants 
Only one person can be assigned a ticket in JIRA. But if you want to add anyone else in TS to keep track/help on a ticket, you can add them as a "watcher" by clicking the eye logo at the top right of the ticket and "add watcher."
![JIRA 3](https://github.com/llsmith305/images/blob/main/Jira_capture_3.png)

If there is someone other than the submitter of the ticket who might want to follow what's happening with the ticket you can add them as a "participant." Participants are people outside of JIRA who will still be able to view the progress of the ticket.
To add particpants, scroll down to "more fields" on the right side of the open ticket and click next to "request particpants."
![JIRA 4](https://github.com/llsmith305/images/blob/main/Jira_capture_4.png)
  

# Archival Planner
## Blue Sheets and Merge Requests
  - Blue Sheets, List2Procs, and GIT merge/push requests are submitted through [this microsoft form](https://forms.office.com/Pages/DesignPageV2.aspx?prevorigin=shell&origin=NeoPortalPage&subpage=design&id=T9WzWMkW00KvCB_KvQlWZjnLCvqsIedCs1g4IqhwWE1UQzRSQUJVM1pNTEtORVVTOVJBWldVMFhMTi4u&topview=Preview), also found as a tab on Wilson SCTS-Archival--General channel in Teams.
  - Once submitted, these tickets automatically populate a task in [the planner](https://tasks.office.com/admin.live.unc.edu/en-US/Home/Planner/#/plantaskboard?groupId=a159b0b7-6c00-46a0-977b-10c99a206261&planId=kmGl8FYePUWMq-0ZMwZYFGQAE4Fn) (also located on Archival's Teams channel) under the "Submitted" column.
  - Laura Smith will manage the workflow for these tickets, but any submitter will be able to check on their tickets' progress in the planner.

## Microsoft Flow
  - The automation from Form to Planner is managed through [a Microsoft Flow.](https://make.powerautomate.com/environments/Default-58b3d54f-16c9-42d3-af08-1fcabd095666/flows/132e7f01-c152-4801-8835-f5157578fa91?v3=true)
  - The TS Blue Sheet Forms to Planner flow connects to the Blue Sheets/GIT Requests Form-->gathers details from this form-->gathers profile details from the submitter of the form-->sends an email alert that there is a new form submission-->creates a task in the Blue Sheets/GIT Requests Planner-->adds details from the submitted Form into the new Planner task.
  - If the Flow fails at any point, it will notify the owner of the Flow (right now, Laura Smith and Dawne).
### Updating Flow Features
Be gentle with Flow. One break in the chain can crash the whole system. There are a couple useful updates when ticket management changes hands though.
#### Adding Co-owners
A current owner of the Flow will need to navigate to the [TS Blue Seet Forms to Planner flow](https://make.powerautomate.com/environments/Default-58b3d54f-16c9-42d3-af08-1fcabd095666/flows/shared/132e7f01-c152-4801-8835-f5157578fa91/details) through Microsoft 365. Flows will be located within the Power Automate app under "My Flows." 

Co-owners can be edited on the right side of the page.
![Flows 5](https://github.com/llsmith305/images/blob/main/Flows_capture_5.PNG)

#### Email Recipients
To update who recieves emails for new form submissions, open the Flow and click on the "Send an email" section. 
![Flows 2](https://github.com/llsmith305/images/blob/main/Flows_capture_2.PNG)

In the pop-up box to the left of the screen, you can change/add email recipients under the "To" field. If you want multiple recipients, be sure to separated email addresses with a semicolon.
![Flows 3](https://github.com/llsmith305/images/blob/main/Flows_capture_3.PNG)

#### Assigned Users
To update who automatically gets assigned new tasks, click on the "Create a task" section of the Flow.
In the pop up, you can add or change the assigned users by adding their UNC emails in the "Assigned User Ids" field at the bottom.
![Flows 4](https://github.com/llsmith305/images/blob/main/Flows_capture_4.PNG)
