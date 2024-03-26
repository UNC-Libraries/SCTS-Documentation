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
