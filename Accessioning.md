# Overview

- Before we begin
- Creating an Accession Record
- Instructions
  - Basic Information
    - Title
    - Identifier
    - Accession Date
    - Content Description
    - General Note
    - Acquisition Type
    - Resource Type
    - Restrictions Apply?
    - ~~Publish?~~
    - Access Restrictions?
    - Access Restrictions Note
    - Use Restrictions
    - Use Restrictions Note
  - Dates
    - Label
    - Expression
    - Type
    - Certainty
    - Removing Dates
  - Extents
    - Portion
    - Number
    - Type
    - Container Summary
    - Removing Extents
  - Agents
    - Role
    - Realator
    - Agent
      - Person Agent Records
      - Family Agent Records
      - Corporate Agent Records
    - Removing Agents
  - Related Resources
    - Resource
    - Removing Related Resources
  - Collection Management
    - Processing Plan
    - Processing Status
  - User Defined
    - Items
    - Monetary
    - New or addition
    - Biographical/historical information
- Tracking Processing and Collection Management Events in ASpace
  - Basic Information
    - Type
    - Outcome
    - Outcome Note
  - Event Date/Time
    - Date/Time Specifier
Agent Links

***

# Before we begin

We enter accession records into ArchivesSpace for all archival material received in Wilson Library. When print materials that require bibliographic cataloging are received as part of a larger archival collection, include a note about the print materials (and where they can be found) in the accession record. Create a ticket with a link to the accession record and submit it to Tickets for Tech Services section of the TS ticketing system. 

**Staff interface:** https://aspace.lib.unc.edu:4433/ 

Login using your Onyen/password

# Creating an Accession Record at the Wilson Special Collections Library

This documentation is supplemental to the documentation provided by ArchivesSpace, and has been adapted for use at the Wilson Special Collections Library. _"Maps to:" notes let you know where you would have entered the same information in AT._

> While entering data you should periodically click **Save Accession**. If any required element is missing, you will be prompted to add that information. Some fields have boilerplate text with instructions. You should delete the instructions as you create the record.

# Instructions

1. On the main toolbar, click **Create** and select Accession. 

2. ArchivesSpace requires two elements for an ArchivesSpace valid accession record. They are Identifier and Accession Date, which serve to document only the accession event.  

Other fields are used for accessions at the Wilson Special Collections Library, and should be filled out if required or as applicable. 

## Basic Information

![screenshot](https://user-images.githubusercontent.com/58087302/76891925-309d8480-6860-11ea-9751-b826c7f28473.png "screenshot example basic info")

### Title (Required by TS)

_Maps to: Title (Basic Information tab)_

The title of the accession will typically, but need not always, match the title of the resource to which the accession belongs. For example, the accession title may be John Smith Diaries, which may become part of the larger Smith Family Papers.  

_Delete the boilerplate instructions!_

When spawning a resource (see below), this field maps to the resource title.

### Identifier (Required by ArchivesSpace)

_Maps to: Accession Number (Basic Information tab)_

Here's how we enter identifiers at the Wilson Special Collections Library: 

- **First component:** select the curatorial department from the drop-down list (GL, NCC, NCCPA, SHC, SFC, UA). 
- **Second component:** this number will autogenerate based on today's date.
- **Third component:** enter the collection number for the collection to which this accession will be added (example: #04534). _If you don't know the collection number at the time of accession, you can leave this component blank and fill it in later._

> Note that we are no longer creating separate accession records for digital items. 

### Accession Date (Required by ArchivesSpace)

_Maps to: Accession Date (Basic Information tab)_

When you create a new accession, this field is automatically filled with the current date, so you may need to edit that date to reflect the actual date of the accession transaction. The accession date in ArchivesSpace is meant to represent the date of the receipt of the materials, which is not necessarily the same as the date the accession record is created and most probably not the date that the contents of the accession were created. 

### Content Description (Required by TS)

_Maps to: Description (Accession Notes tab)_

A description of the document types and topical contents of the accession. When spawning a resource, this field maps to the main level scope and content note. 

_Delete the boilerplate instructions!_

### General Note

_Maps to: General Accession Note (Basic Information tab)_

Intended for notes about the acquisition or processing of the accession, and not about the accession itself. Can used as a place to record temporary locations. (examples: 206_7a.1 or BD lab). 

> Note that we will stop using this field to record temporary locations once we start using ArchivesSpace as our locations database. 

_Delete the boilerplate instructions!_

### Acquisition Type (Required by TS)

_Maps to: Acquisition Type (Accession Notes tab)_

Choose from a drop-down list. A categorical descriptor for the type of acquisition. We typically select _gift, purchase, or transfer._

### Resource Type (Required by TS)

_Maps to: Resource Type (Basic Information tab)_

Choose from a drop-down list. A list of terms for categorizing resources into basic types. We typically select _Collection, Papers, or Records._

### Restrictions Apply?

_Maps to: Restrictions Apply (Acknowledgements, Restrictions & Processing Tasks tab)_

A selected check box indicates that restrictions apply. The restrictions can be explained using the Access Restrictions Note and/or Rights sub-records, described elsewhere below. 

### Publish?

Do not check this box. Just leave it alone. Pretend you never saw it.

### Access Restrictions

_Maps to: Access Restrictions (Acknowledgements, Restrictions & Processing Tasks tab)_

A selected check box indicates that access to the materials is restricted. 

### Access Restrictions Note

_Maps to: Access Restrictions Note (Acknowledgements, Restrictions & Processing Tasks tab)_

A statement indicating what materials in the accession have restrictions on access, what the authority of the restriction is, and for how long the restriction will be in effect. Additional information may also be recorded in a Rights sub-record. 

### Use Restrictions

_Maps to: Use Restrictions? (Acknowledgements, Restrictions & Processing Tasks tab) _

A selected check box indicates that there are use restrictions for materials in the accession. The restrictions can be explained using the Use Restrictions Note and/or Rights sub-records, described below. 

### Use Restrictions Note

_Maps to: Use Restrictions Note  (Acknowledgements, Restrictions & Processing Tasks tab)_

A statement indicating which materials have use restrictions, how the materials can be used, what the authority of the restriction is, and for how long the restriction will be in effect. Additional information may also be recorded in a Rights sub-record.

## Dates

_Maps to: Date Expression (Basic Information tab)_

This sub-record identifies and records the date(s) that pertain to the creation, assembly, accumulation, and/or maintenance and use of the materials being described. The required fields are **Label, Type,  Date Expression.**

One Date sub-record will automatically appear as part of the accession record template. To create additional Date sub-records, click **Add Date** on the right side of the screen.

![screenshot](https://user-images.githubusercontent.com/58087302/76894777-2b8f0400-6865-11ea-800e-ed6f1e7e2fd5.png "screenshot example dates")

### Label (Required by ArchivesSpace)

Choose from a drop-down list. Describes the type of activity that the date signifies. You will most likely always select _Creation._

### Expression (Required by TS)

The date or date range of the materials in the accession. Some examples: 1968; 1979-1993; 1785-1960; bulk 1916-1958; 1827; circa 1870-1879; 1906 March 1; undated. 

_Delete the boilerplate instruction!_

### Type (Required by ArchivesSpace)

Choose from a drop-down list. Indicate the type for normalized date information, either a single date or a date range (inclusive or bulk). The default is "Inclusive." 

### Certainty

Choose from a drop-down list. Indicate the level of confidence for the information given in a date statement. This information is optional and should only be added when you are qualifying date information as potentially uncertain based upon the description or cataloging rules in use.  

### Removing a Date sub-record:

1. Find the Date sub-record that is to be deleted.
2. Click on the **X** in the upper right corner of the Date sub-record link. 
3. Click on the **Confirm Removal** option to remove the Date sub-record from the accession record, or on the **Cancel** option to retain the sub-record. 
4. Click on **Save** in the context record to save the accession record with the Date sub-record removed. 

## Extents

_Maps to: Extent (Basic Information tab)_

This sub-record is used for recording the extent (items, volume, or containers) of the described materials. The required fields are Portion, Number, and Type. 

**You may add as many extent records as needed. This means that you can record physical and digital extents in the same record. Hooray! To do this, you will need to create more than one sub-record using the steps below.**

One Extent sub-record will automatically appear as part of the accession record template. To add an additional Extent sub-records, click **Add Extent** on the right side of the screen. 

![screenshot](https://user-images.githubusercontent.com/58087302/76895739-f2579380-6866-11ea-93c0-b9509988dba7.png "screenshot example extent")

### Portion (Required by ArchivesSpace)

_Maps to: This is a new feature that does not map to AT_

Used to specify whether an extent statement relates to the whole or part of a given accession. Choose part or whole from the drop-down list. If you are recording multiple extents (for example, if you have 1 box of papers and 1 hard drive), you will need to create multiple sub-records. 

### Number (Required by ArchivesSpace)

_Maps to: Extent number (Basic Information tab)_

 A numeric value for indicating the number of units in the extent statement, e.g., 5, 11.5, 245. Used in conjunction with Type (below) to provide a structured extent statement. 
 
 ### Type (Required by ArchivesSpace)
 
 _Maps to: Extent number (Basic Information tab)_
 
 A term indicating the type of unit used to measure the extent of materials described (examples: items, linear feet, gigabytes). Choose from a drop-down list.  
 
 ### Container Summary (Required by TS)
 
 _Maps to: Container Summary (Basic Information tab)_
 
Serves to describe the logical or physical parts of a multi-level resource or digital object that makes up an aggregation of archival materials. Example of use: if the Number and Type are 10 linear feet, then the container summary might be used to record the actual number of containers (10 boxes and 4 flat files) 
 
_Delete boilerplate instructions!_

### Removing an Extent sub-record:

1. Find the Extent sub-record that is to be deleted.
2. Click on the **X** in the upper right corner of the Extent sub-record.
3. Click on the **Confirm Removal** option to remove the Extent sub-record, or on the **Cancel** option to retain the sub-record.
4. Click on **Save** in the context record to save the context record with the Extent sub-record removed.

## Agent [a.k.a. Names] Links

_Maps to: Names & Subjects tab_

This sub-record enables associating an agent as a creator, source, or subject to the materials being described, as a rights holder to a rights statement, as an agent responsible for a recorded event, and to other agents. 

> Note that we will be using agent records much more comprehensively in the future!

**Linking agent record(s) to a material description record:**

One or more agent records may be linked to a material description record as either a creator, a source, or a subject of the materials being description. You may add as many agent links as needed. Also, the same agent record may be linked to the same context record multiple times as long as the value recorded for **Role** and **Relator** are different for each link occurrence. In other words, an agent record may not be linked two or more times to the same context with the same **Role** value and same **Relator** value. 

To link an agent record to a material description record, click **Agent Links** on the left navigation bar and then click **Add Agent Link** on the right side of the screen. 

![screenshot](https://user-images.githubusercontent.com/58087302/76896528-5d559a00-6868-11ea-936c-0ba1981f089b.png "screenshot example agent")

### Role (Required by ArchivesSpace)

_Maps to: Function (Names & Subjects tab)_

Choose from drop-down list. An indication of what function (creator, source, or subject) the agent has in regards to its link to a certain material description record. Note that if you choose a Role=Creator, the screen will present a **Title** field. _You do not have to fill in the **Title** field._

### Realator (_Very_ optional)

_Maps to: Role (Names & Subjects tab) Isn't that confusing?_

Choose from drop-down list. A more specific indication of what role the agent has in respect to the materials being described. For example, an agent may be linked as a creator to a record, but with the more specific role of "illustrator" or as the source to a record, but with the more specific role of "donor."  

### Agent (Required by ArchivesSpace)

_Maps to: Name Lookup (Names & Subjects tab)_

For identifying the agent related to the material described in the record. Agents may be searched using auto-complete, using a browse function, or, if need be, may be created on demand. 

- To select an agent using the auto-complete function simply start typing the name of an agent in the agent box to find an agent in the agent index. The system will present you with names matching the string you have keyed. Select the name that matches the name you want to link to the materials being described. 

![screenshot](https://user-images.githubusercontent.com/58087302/76898431-136eb300-686c-11ea-8227-227ad61b9159.png "screenshot agent dropdown 1")

- To select an agent using the Browse function, click on the drop down arrow by the agent box and select **Browse**. 

![screenshot](https://user-images.githubusercontent.com/58087302/76899353-b5db6600-686d-11ea-967f-09fc5e887cbb.png "screenshot agent dropdown 2")

- Search for and select the desired agent(s) on the resulting screen. Multiple agents can be selected and linked to the context record providing the agents all have the same role and relator values.

- Click **Link to Agent** to add the agent(s) to the context record for the material being described and to close the Browse Agent screen. 

- If you cannot find the name you need, click **Cancel** or the **X** at the upper right to exit the Browse Agents screen without selecting a name. 

![screenshot](https://user-images.githubusercontent.com/58087302/76899447-ea4f2200-686d-11ea-89e9-136f785b74f8.png "screenshot agent dropdown 3")

- To create a new agent record, click on the drop down arrow by the agent box, select **Create**, and then select the type of agent record you wish to create. A minimal agent record may be created by filling in only the required fields. The minimal record can be enhanced later by adding additional information in other fields and sub-records. 

![screenshot](https://user-images.githubusercontent.com/58087302/76900165-30f14c00-686f-11ea-8bc4-887de85d0a8f.png "screenshot agent dropdown 4")

- Each agent type has several required fields you must complete in order to save a new agent record to the database. Required fields are marked with red asterisks. In addition to required fields, there are several conditionally required fields. These fields are marked with gray asterisks. The conditions under which these fields are required are explained in the fields’ tooltip, which is accessed by hovering your cursor over the gray asterisks. 

![screenshot](https://user-images.githubusercontent.com/58087302/76900216-4cf4ed80-686f-11ea-8159-6af701bfaf2e.png "screenshot agent dropdown 5")

- Click **Create and Link to Agent** when you have finished the below, and completed the data entry. 

#### Person agent records:

- **Primary Part of Name** (required by ArchivesSpace) 
- **Rest of Name** (required by TS unless there's a really compelling reason) 
- **Source or Rules** (conditionally required) 
- **Sort Name** (automated if selected) 
- **Name Order** (default value of "indirect" provided; you may change to "direct") 

#### Family agent records:

- **Family Name** (required by ArchivesSpace) 
- **Source or Rules** (conditionally required) 
- **Sort Name** (automated if selected)

#### Corporate Entity agent records:

- **Primary Part of Name** 
- **Source or Rules** (conditionally required) 
- **Sort Name** (automated if selected) 

### Removing a link to an Agent Record:

1. Find in the agent record link that is to be deleted. 
2. Click on the **X** in the upper right corner of the agent record link. 
3. Click on the **Confirm Removal** option to remove the link, or on the **Cancel** option to retain the link. 
4. Click on **Save** to save the context record with the agent link removed. 

## Related Resources (a.k.a. Collections)

_Maps to: Resources Linked to this accession (Basic Information tab)_

This field allows you link an accession to an existing resource record in your repository. The **Resource** field is required. You may link as many resource records to an accession as necessary. 

To link a related resource to an accession record, click **Related Resources** on the left navigation bar and then click Add Related Resource on the right side of the screen. 

![screenshot](https://user-images.githubusercontent.com/58087302/76900784-65193c80-6870-11ea-9071-5e886994e39b.png "screenshot related resources")

### Resource (Required by ArchivesSpace)

Two selection options: 1) start typing to filter existing resources and autocomplete the field; 2) use the down arrow to browse existing resources. 

- To select a resource using the auto-complete function simply start typing the resource title in the Resource box. The system will present you with matching options as you type. Select the resource record you want to link the accession to and it will populate the Resource box. 

- To select a resource record using the Browse function, click on the down arrow by the agent box and select Browse. Search for and select the desired resource record on the resulting screen. Click **Link to Resource** to add the resource to the accession record and close the Browse Resources screen. 

- If you cannot find the resource you need, click Cancel or the X at the upper right to exit the Browse Resources screen without selecting a resource. You will need to spawn a new resource record from the accession record. 

- To spawn a resource record, click **Spawn**, and select **Resource**. The new editable resource record displays. 

> REMINDER THAT IN ORDER TO SPAWN YOU HAVE TO HAVE SAVED YOUR ACCESSION RECORD ALREADY?

![screenshot](https://user-images.githubusercontent.com/58087302/76984065-b8dd6180-6914-11ea-96d0-0f930db25a2b.png "screenshot related resources 2")

- The system will then open a new resource record containing information from the accession record. Note that the screen also has a **Return to Accession** button. This enables you to back out of creating the resource and is only available until you save the resource record. 

![screenshot](https://user-images.githubusercontent.com/58087302/76985062-0dcda780-6916-11ea-95a7-f30277be3f63.png "screenshot related resources 3")

- Add the additional required fields to the resource record, if they have not already carried over from the accession record. 

> SOME CARRIED OVER, SOME DID NOT. IS THERE A RHYME OR REASON? 

- The required fields are: 

  - **Title:** Open text field. The title assigned to the resource.
  - **Identifier:** Open text field. The collection number.
  - **Level of Description:** Choose from a drop-down list. Indicates the hierarchical level of the materials being described. We typically use _Collection, Papers, or Records._
  - **Dates fields:** See Dates sub-record documentation above.
  - **Extenets fields:** See Extents sub-record documentation above.
  
- Click **Save Resource**.

### Removing a link to a Relate Resource record

1. Find the relevant accession record, and click Edit to edit the record, if not currently in edit mode. Navigate to the related resource link that is to be removed from the record. 
2. Click on the **X** in the upper right corner of the related resources record link. 
3. Click on the **Confirm Removal** option to remove the link, or on the **Cancel** option to retain the link. 
4. Click on **Save Accession** to save the record with the link removed. 


## Collection Management

This sub-record is used to add staff-only information about the processing of materials described in an accession. Only one collection management record may be added per accession.  

![screenshot](https://user-images.githubusercontent.com/58087302/76985970-694c6500-6917-11ea-8c11-25b4101e665a.png "screenshot collection management")

### Processing Plan (Required by TS)

_Maps to: Processing Plan (Acknowledgements, Restrictions & Processing Tasks tab)_

Open text field. For recording a plan for processing of the archival unit. We typically use _Acc2Proc_ or _Intake_. 

_Delete the boilerplate instructions!_

### Processing Status

_Maps to: Processing Status (Acknowledgements, Restrictions & Processing Tasks tab)_

Choose from drop-down list. We typically do not use this field until the accession has been **Processed**.


## User Defined

User-defined fields are used to record additional information about materials not supported in other sections of the accession record. 

Please note that there are several user defined fields that we did not migrate from AT. The number of items, which used to be recorded in a user defined field, should now be recorded as an extent. 

![screenshot](https://user-images.githubusercontent.com/58087302/76986346-ee377e80-6917-11ea-9b2b-19ea9b8cf172.png "screenshot user defined")

### Items

_Maps to: Items (User defined fields tab)_

Used to record the approximate number of items in an accession. 

_Delete the boilerplate instructions!_

### Monetary

_Maps to: Monetary (User defined fields tab)_

Used to record how much money was paid for an accession, if applicable.

### New or addition

_Maps to: New or addition (User defined fields tab)_

Used to record whether an accession is creating a new collection, or adding to an existing collection. 

_Delete the boilerplate instructions!_

### Biographical/historical information

_Maps to: Biographical/historical information (User defined fields tab)_

Used to record biographical and historical information related to an accession and its agents. In the future, we might record some of this information in the agent records. 

_Delete the boilerplate instructions!_

***

Once these instructions have been completed, click **Save Accession**. If any required element is missing, you will be prompted to add the information.


# Tracking Processing and Collection Management Events in ASpace 

Events represent a specific action that one or more people undertook in relation to an accession at a specific date and time (or in a range of dates and times). You can create a variety of event records, including (but not limited to): 

- Processed
- Ingested
- Agreement Sent
- Agreement Received
- GIK Report Submitted

To add an event record to an accession record:

1. Find the accession record you want to edit. You can browse or search. 
   - To browse, on the main toolbar, click **Browse** and select **Accessions**. A listing of all the accession records in the repository displays.
   - To search, on the main toolbar, type your search query into the **Search** box.
2. Next to the accession record you want to edit, click **Edit**.
3. At the top of the accession record, click **Add Event**.
4. Select the type of event from the drop-down list.
5. Click **Add Event**.
6. Follow the instructions below to complete the record.

## Basic Information

![screenshot](https://user-images.githubusercontent.com/58087302/76987140-14115300-6919-11ea-899a-89e77bbf2b6a.png "screenshot for Aspace basic info")

### Type (Required by ArchivesSpace)

Choose from drop-down list. The default is "Processed." 

### Outcome (Very optional)

Choose from drop-down list. Describe the overall result of the event in terms of success, partial success, or failure. Recommended practice is to define events with sufficient granularity that each event has a single outcome and to use a controlled vocabulary that a system can act upon automatically. More detail about the outcome may be recorded in an Outcome Note.  

### Outcome Note (Very optional)

Open text field. Provide a detailed description of the result or product of the event. This field may be used to record error and warning messages issued by a program involved in the event or to record a pointer to an error log. 

## Event Date/Time

This sub-record is required. Only one date may be associated with an event record. 

### Date/Time Specifier (Required by ArchivesSpace)

Choose from drop-down list. Indicates the type of date is associated with this event. The default is "Date Subrecord." 

**If Date Sub-record is chosen for the Date/Time Specifier**, the required fields are Label and Type.

- **Label (Required by ArchivesSpace)** Choose from drop-down list. Use to describe the type of activity the date signifies. The default is "Event." 

- **Expression (Required by ArchivesSpace)** Open text field to record the date the event occurred. _Delete the boilerplate instructions!_

- **Begin (Not Required)** Enter the date when the event began.

- **End (Not Required)** Enter the date when the event ended.

- **Type (Required by ArchivesSpace)** Choose from a drop-down list. Indicate the type for normalized date information, either a single date or a date range (inclusive or bulk).  

- **Certainty (Not Required)** Choose from a drop-down list. Indicate the level of confidence for the information given in a date statement. This information is optional and should only be added when you are qualifying date information as potentially uncertain based upon the description or cataloging rules in use. 

- **Era (Not Required)** Choose from a drop-down list. Period during which years are numbered and dates reckoned, such as B.C. or C.E. The value "ce" is the default.  

- **Calendar (Not Required)** Choose from a drop-down list. System of reckoning time, such as the Gregorian calendar or Julian calendar. The value "Gregorian" is the default. 

**If UTC Timestamp is chosen for the Date/Time Specifier,** the required field is UTC Timestamp. 

- **UTC Timestamp (Required by ArchivesSpace)** A specific timestamp, with full date and time information, about when the event occurred. By default, the application assumes that the timestamp is in UTC: YYYY-MM-DD HH:MM:SS. 


# Agent Links

To link an agent to an event record, click Add **Agent Link** on the right side of the screen. 

The required fields are **Role** and **Agent**.

- **Role (Required by ArchivesSpace)** Choose from drop-down list. Indicate what function (collecting unit, processor, etc.) the agent has in regards to the event. 

- **Agent (Required by ArchivesSpace)** Choose from drop-down list. Select the agent (personal or corporate name) that is related to the event. Agents may be searched using auto-complete, using a browse function, or may be created on demand. 

  - If linking the name of a collecting unit, please use one of the following authorized records: 
  
    - University of North Carolina at Chapel Hill. Library. North Carolina Collection  
    - University of North Carolina at Chapel Hill. Library. Rare Book Collection  
    - University of North Carolina at Chapel Hill. Library. Southern Folklife Collection  
    - University of North Carolina at Chapel Hill. Library. Southern Historical Collection 
    - University of North Carolina at Chapel Hill. Library. University Archives and Records Service  
    
  - If linking the name of a processor, please use the existing record, or create a new record if needed (see "Agent [a.k.a. Names] Links" above). 
