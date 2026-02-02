Created by Dawne Lucas in August 2025 

# Creating Finding Aids in ArchivesSpace at UNC-Chapel Hill

These are instructions for creating finding aids using ArchivesSpace, Pipette, and ArcLight (Archy) at the Wilson Special Collections Library at UNC-Chapel Hill. This documentation is supplemental to the documentation provided by ArchivesSpace, and has been adapted for use at the Wilson Special Collections Library. Some of the procedures described in this documentation differ from procedures followed at other institutions. It is therefore important that you read these procedures carefully, even if you already have experience using ArchivesSpace.

# Overview

 - [Introduction: ArchivesSpace, ArcLight (Archy), and Pipette](#introduction-archivesspace-arclight-archy-and-pipette)
 - [ArchivesSpace Terminology](#archivesspace-terminology)
 - [Finding Aid Creation](#finding-aid-creation)
   - [Resource Record Structure](#resource-record-structure)
   - [Collection-level Fields and Notes](#collection-level-fields-and-notes)
     - [Basic Information](#basic-information)
     - [Languages](#languages)
     - [Dates](#dates)
     - [Extents](#extents)
     - [Finding Aid Data](#finding-aid-data)
     - [Revision Statements](#revision-statements)
     - [Related Accessions](#related-accessions)
     - [Agent Links](#agent-links)
     - [Subjects](#subjects)
     - [Notes](#notes)
       - [Abstract](#abstract)
       - [Processing Information](#processing-information)
       - [Biographical and Historical Note](#biographical-and-historical-note)
       - [Scope and Content](#scope-and-content)
       - [Restrictions to Access](#restrictions-to-access)
       - [Restrictions to Use](#restrictions-to-use)
       - [Copyright Notice](#copyright-notice)
       - [Preferred Citation](#preferred-citation)
       - [Acquisitions Information](#acquisitions-information)
       - [Separated Materials](#separated-materials)
     - [External Documents](#external-documents)
     - [Rights Statements](#rights-statements)
     - [Metadata Rights Declarations](#metadata-rights-declarations)
     - [Instances](#instances)
     - [Deaccessions](#deaccesions)
     - [Collection Management](#collection-management)
     - [Classifications](#classifications)
     - [User Defined](#user-defined)
   - [Adding Series, Subseries, and File Level Archival Objects](#adding-series-subseries-and-file-level-archival-objects)
     - [Rapid Data Entry](#rapid-data-entry)
     - [Load via Spreadsheet](#load-via-spreadsheet) 
   - [Revising Series, Subseries, and File Level Archival Objects](#revising-series-subseries-and-file-level-archival-objects)
     - [Manual data entry](#manual-data-entry)
     - [Bulk Archival Object Updater](#bulk-archival-object-updater) 
   - [Finding Aid Publication Workflow](#finding-aid-publication-workflow)
   - [Finding Aid Checklist](#finding-aid-checklist)
  
   ***
   
# Introduction: ArchivesSpace, ArcLight (Archy), and Pipette

Here’s the very tl;dr summary of the difference between ArchivesSpace, ArcLight (Archy), and Pipette:

 - **ArchivesSpace:** Staff-only interface used to create finding aids.
   - Staff interface: https://aspace.lib.unc.edu:4433/
   - Login using your ONYEN password.
   - Don't have an account? Contact Dawne.
 - **ArcLight (Archy):** Public-facing interface used to display finding aids.
   - https://finding-aids.lib.unc.edu/
   - UNC's version of ArcLight was named "Archy" (ArcLight at UNC-Chapel Hill) by Library Software Applications Developer Dean Farrell. "Archy" is UNC-specific, and the name is not used by other institutions using ArcLight.
 - **Pipette:** Staff-only interface used to preview and publish finding aids in ArcLight.
    - Preview: https://finding-aids-qa.lib.unc.edu/admin
    - Contact Dawne if you need access.   
    - NB: Content published to ArcLight is tracked via Git/Sourcetree, but TS-Archival does not interact with it. 
    - This is a UNC-specific application.
     
Remember: these are merely new tools for creating and displaying finding aids and do not replace our best practices for archival description, including:

 - <a href="https://github.com/UNC-Libraries/SCTS-Documentation/blob/main/Descriptive%20Elements.md">Descriptive Elements</a>
 - <a href="https://github.com/UNC-Libraries/SCTS-Documentation/blob/main/Style%20Guide.md">Style Guide</a>

# ArchivesSpace Terminology

ArchivesSpace comes with its own jargon that might be new to you. Here are some terms that you should learn to love:

 - **Archival object:** Unit of archival description, such as a folder title.
   - Archival objects map to components (```<c0x>```) in EAD. 
 - **Instances:** Instances link archival objects to their physical containers (container instance) or digital files (digital object). 
   - ArchivesSpace is not a digital content repository and does not store digital files (just as it doesn’t store physical boxes). Digital objects merely serve as a link between ArchivesSpace and CONTENTdm, the DCR, or anywhere else digitized content might be stored.
 - **Resource:** Another term for "collection." Finding aids are generated from ArchivesSpace resource records.

# Finding Aid Creation

> These workflows are new to us and might change over time as ArchivesSpace changes over time and as we become more familiar with how to use it. If you see something in the instructions below that appears incorrect or just isn’t working for you, please contact Dawne ASAP.
>
> Furthermore, these workflows document UNC-specific procedures and do not cover everything there is to know about ArchivesSpace. Additional ArchivesSpace documentation is available via the <a href="https://archivesspace.atlassian.net/wiki/spaces/ADC/pages/917045261/ArchivesSpace+Help+Center">ArchivesSpace Help Center</a>, accessible via your Confluence account. Links to the ArchivesSpace Help Center are occasionally listed in the documentation below.

We create finding aids in ArchivesSpace using resource records. Resource records provide a structure to archival description similar to that found in our legacy EAD templates. Most fields in a resource record map to an EAD field, allowing end users to download a structured PDF version of the finding aids and (for anyone who wants it) the XML encoding. 

There are two ways to create resource records in ArchivesSpace. One way is to create a resource record within the Resource module. The other way is to "spawn" a resource record from an existing accession record. Both ways are subject to the same record requirements.

NB: Since we are using ArcLight instead of the ArchivesSpace Public User Interface, edits made to resource records will not automatically appear to the public. However, lengthy edits should be worked on outside of ArchivesSpace in order to avoid merge conflicts. More about that later!
 

## Resource Record Structure

Information in resource records is recorded in 18 different sections. You can see the sections listed in a menu on the left side of each resource record.

<img width="1416" height="609" alt="Picture1" src="https://github.com/user-attachments/assets/c4738500-624a-4c9c-8330-45cb13d27c8a" />

 - **1.	Basic Information:** As the name suggests, this is where basic information about the collection, such as collection title and collection number are recorded.
 - **2.	Languages:** The languages and scripts represented in the material(s) described.
 - **3.	Dates:** The dates(s) represented in the material(s) described.
 - **4.	Extents:** The size of the materials described.
 - **5.	Finding Aid Data:** Information about the finding aid, as opposed to the materials described.
 - **6.	Revision Statements:** Description(s) of revision(s) made to the finding aid.
 - **7.	Related Accessions:** Used for linking associated accessions to the resource record.
 - **8.	Agent Links:** Used for linking agent (name) records to the resource record.
 - **9.	Subjects:** Used for linking subject records to the resource record.
 - **10.	Notes:** This is where you enter all of various collection-level notes, including the Scope and Content note and the Biographical and Historical note. 
 - **11.	External Documents:** Links to pertinent information stored outside of ArchivesSpace, such as appraisal reports and spreadsheets. These will not display in the finding aid.
 - **12.	Rights Statements:** Used to record information about the rights status of the material being described.
 - **13.	Metadata Rights Declarations:** Used to record rights statement for archival description and archival authority records.
 - **14.	Instances:** Used to link containers (boxes, etc.) and information about digitized content.
 - **15.	Deaccessions:** Used to record information about materials that have been deaccessioned from the collection.
 - **16.	Collection Management:** Internal-only information about how the materials described will be or have been processed.
 - **17.	Classifications:** We are using classifications to record collecting units. This field allows faceting by collecting unit in ArcLight. Finding aids without an assigned classification cannot be published in ArcLight.
 - **18.	User Defined:** These fields are for internal purposes only. They do not display in ArcLight.

We will discuss each one of these sections in more detail later in this documentation. First, let’s discuss the fields that must be filled out in order to create a collection level record (CLR).

## Collection-level fields and notes

All resource records must have the following data, which contain red asterisks in ArchivesSpace:

 - Title
 - Identifier (a.k.a. Collection Number)
 - Level of Description (defaults to "Collection")
 - Languages sub-record
 - Date sub-record
 - Extents sub-record
 - Finding Aid Data ("Language of Description" and "Script of Description")
   
Resource records will not save unless these fields have been filled out. You should not add series, subseries, folders, boxes, etc., until these fields have been filled out.

Let’s go through each section of the collection level resource record. **Please note that except for the six fields listed above, you do not need to add all this information to a resource record at once.** 

You'll notice some fields in ArchivesSpace that aren't mentioned in these instructions. Rest assured that you don't have to worry about them.

When applicable, the EAD tags that fields map to are included in these instructions. This information is useful to staff members who have used EAD in the past. Don’t worry about them if you’re not familiar with EAD.

### Basic Information

<img width="693" height="320" alt="Picture2" src="https://github.com/user-attachments/assets/0a550fd0-4989-414c-b4f8-6955652859a5" />

 - **Title:** Collection title.
   - **Maps to:** ```<unittitle>```
   - **Example**: G. K. Butterfield Papers, 1942-2021
   - **Required to save record**
   - Note: Include the date, even though you will repeat it in the "Date" sub-record.

 - **Identifier:** Collection number. This number must be unique. You cannot create more than one resource record with the same identifier.
   - **Maps to:** ```<unitid>```
   - **Example:** 60010
   - **Required to save record**

- **Automatically Generate Slug?:** This box should already be checked.

- **Level of Description:** This value is automatically set to "Collection." If needed, you can change this value from the drop menu, although "Collection" should almost always suffice.
  - **Maps to:** ```<archdesc>```
  - **Required to save record**

- **Resource Type:** Select "Collection," "Papers," or "Records" from the drop menu, as appropriate.
  - Generally speaking, SFC = "Collection"; SHC = "Papers"; UARMS = "Records"

 - **Publish?:** This box needs to be checked in order for the finding aid to be indexed and published in ArcLight, including previewing on finding-aids-qa.

 - **Restrictions Apply?**: Check this box if the collection has any access or use restrictions.

 - **Repository Processing Note:** This is an optional field to record internal notes. It will not be seen by the public, even if the record is published.

### Languages 
Maps to: ```<langmaterial>```

 - **Language:** The language(s) represented in the materials. This value is automatically set to "English." This is usually correct!
   - **Maps to:** ```<langmaterial><language>```
   - **Required to save record**
   - For the small number of times when the default is not adequate, you can do one of the following: 
   - Change the language from "English" to whatever the appropriate language is. 
   - Add additional languages/scripts using the "Add Language" button available in the top right corner OR the bottom of the "Languages" section. You might have to hover to see the button at the bottom.


<img width="690" height="300" alt="Picture3" src="https://github.com/user-attachments/assets/ef1fdd00-06e4-450f-9aeb-2d0025dbcd55" />

 - **Language of Materials Note**: This value is automatically set to "Materials in English." This is usually correct!
   - **Maps to:** ```<langmaterial><language>```
   - For the small number of times when the default is not adequate, you can change the language from “English” to whatever the appropriate language(s) is/are.
  
 - **Script:** The script(s) represented in the materials (i.e., Latin, Gothic, Greek, etc.). This value is automatically set to "Latin." This is usually correct!
   - **Maps to:** ```<language>```
   - For the small number of times when the default is not adequate, you can change the script from “Latin” to whatever the appropriate script is.
  
### Dates

Maps to: ```<unitdate>```

<img width="698" height="242" alt="Picture4" src="https://github.com/user-attachments/assets/38630575-ed31-41ab-9a5a-a4eaf5ba5075" />

 - **Label:** This field defaults to "Creation," but can be changed via the drop menu if needed.
   - Required to save record
  
- **Expression:** The date or date range.
  - **Typically maps to:** ```<unitdate type="inclusive">```
  - Required to save record if the "Begin" and "End: fields are blank (see below). It is strongly recommended that you fill out the "Expression" field in addition to the "Begin" and "End" dates.
  - **Examples:**
    - 1985
    - November 1985
    - 1985-1990
    - circa 1985

- **Type:** This field defaults to "Inclusive," but can be changed via the drop menu if needed.
  - Required to save record.
 
 - **Begin and End:** Use these fields to record normalized dates.
  - **Maps to:** ```<unitdate type="normal">```
  - Required to save record if the “Expression” field is blank (see above). It is strongly recommended that you fill out the “Begin” and “End” dates as well as the “Expression” field.
  - Record single dates in the “Begin” field and leave the “End” field blank.
  - **Examples:**
    - 1985
      - Record in “Begin” field and leave “End” field blank.
    - 1985-1990
      - Record 1985 in the “Begin” field and 1990 in the “End” field.
        
**Pro tip:** You can add a bulk date by clicking the “Add Date” button in the top right corner OR the "+" at the bottom of the "Dates" section. You might have to hover to see the "+" at the bottom. Select "Bulk Date" for the "Type.”" 

**Note:** It's important to add the date, even though you are also recording the date in the “Title” field under “Basic Information.” 
  

### Extents

Maps to: ```<extent>```

<img width="714" height="242" alt="Picture5" src="https://github.com/user-attachments/assets/46e8c1d6-acad-4c88-a443-01824b237247" />

 - **Portion:** This field defaults to "Whole," but can be changed to "Part" via the drop menu if needed.
   - Required to save record.

- **Number:** The extent of the collection. It does not have to be a whole number.
  - Required to save record.
  - To be consistent with the nearly 6,200+ finding aids ingested into ArchivesSpace, it is strongly recommended to record the number of items in this field.
    - **Examples:**
      - 1
      - 3600
  

 - **Type:** Recommend setting to "items," but other values can be used as needed (say, "Gigabytes" if the collection is digital only).
   - Required to save record.
  
- **Container Summary:** Add additional extent information here. This will usually be the number of linear feet.
  - **Example:** 0.5 linear feet
  - Not required to save record, but strongly suggested to <a href="https://github.com/UNC-Libraries/SCTS-Documentation/blob/main/Descriptive%20Elements.md#extent">conform to our practices.</a> 


**Pro tip:** You can add more extents by clicking the "Add Extent" button in the top right corner OR the "+" at the bottom of the "Extents" section. You might have to hover to see the "+" at the bottom.  Select "Part" for the "Portion." 

### Finding Aid Data

Maps to: ```<eadheader>```

Information in these fields will not be seen by the public, even if the rest of the record is published. 

<img width="707" height="367" alt="Picture6" src="https://github.com/user-attachments/assets/29ee8188-392d-4033-b576-da6278890e7c" />

You can ignore any field not mentioned below.

- **EAD ID:** The EAD ID is the same as the collection number. 
  - **Maps to:** ```<eadid>```
  - Not required to save record, **but please do fill it out.** You cannot upload spreadsheets or index in Archy without this field (more on that later).
  - **Example:** 60010

- **Finding Aid Title:** The Finding Aid Title is the same as the collection title.
  - **Maps to:** ```<titleproper>```
  - **Example:** Dawne Howard Lucas Papers

- **Finding Aid Date:** The date the finding aid was completed.
  - **Maps to:** ```<profiledesc><creation>```
  - **Example:** August 2021
 
- **Finding Aid Author:** The name of the person who completed the finding aid.
  - **Maps to:** ```<profiledesc><creation>```
  - **Example:** Nancy Kaiser
 
 - **Description Rules:** Please don’t populate this field. At the moment it causes display issues in Archy.

 - **Language of Description Note:** This field defaults to "English." Unless you are creating a finding aid in another language (unlikely!), you will never need to change this default.
   - **Maps to:** ```<langusage><language>```
   - Required to save record

- **Sponsor:** This field will usually be blank. It can be used to record sponsor information when applicable.
  - **Maps to:** ```<sponsor>```
  - **Example from finding aid ingested from EAD:** Funding from the State Library of North Carolina supported the encoding of this finding aid. Funding from the Terry and Laurie Sanford Library Fund supported the digitization of this collection.
 
- **Finding Aid Status:** Use the drop menu to choose the correct status. Make sure to set it to "Completed" once it is done!
  - **Maps to:** ```<eadheader findaidstatus>```
  - If working on a new finding aid, use the status "In Progress." When a resource record is set to this status, it cannot be published via Pipette.
  - If revising an existing finding aid, use the status "Under Revision." When a resource record is set to this status, it cannot be published via Pipette.
  - Make sure to set the status to "Completed" once you are done! Changing the status will allow the resource record to be published via Pipette.
 
- **Finding Aid Status Published?:** This box should remain unchecked.

- **Finding Aid Note:** You can use this note to record any extraneous internal information about the finding aid. Remember, these notes will not be seen by the public. 
  - **Maps to:** ```<notestmt>```
  - For finding aids ingested from EAD, this field is populated with "This finding aid is NCEAD compliant."
    
### Revision Statements

Maps to: ```<revisiondesc>```

This field is also part of the ```<eadheader>``` and will not be seen by the public, even if the rest of the record is published. But it's still very important!
When you revise a resource record, add a Revision Statement by clicking the "Add Revision Statement" button.

You will then see the following fields:

- **Revision Date:** The date the revisions were made. You can use this format: ```MONTH YEAR```
  - Required to save record.
  - **Example:** August 2025

- **Revision Description:** An explanation of who made the revision and why.
  - Required to save record
  - **Example:** Revised by Jodi Berkowitz to correct biographical information.

- **Publish?:** Since this field won’t display regardless, there’s no need to worry about this box.

<img width="711" height="165" alt="Picture7" src="https://github.com/user-attachments/assets/a7364b7b-fb0c-4f18-a651-b9136975df66" />

**Pro tip:** You can add more Revision Statements by clicking the "Add Revision Statement" button in the top right corner OR the "+" at the bottom of the "Revision Statements" section. You might have to hover to see the "+" at the bottom.  

### Related Accessions

This field will list any accessions linked to this resource record. These links do not appear in the published finding aid in Archy. They are usually linked from the accession record, so you shouldn't have to do anything here.

<img width="751" height="127" alt="Picture8" src="https://github.com/user-attachments/assets/22d561a4-a14a-45d2-bd74-9e20d8d6e0b4" />

IF you do need to link an accession record for some reason, click on the "Add Related Accession" button, search for the accession, and link it to the resource record. 

**Pro tip:** You can add more Related Accessions by clicking the "Add Related Accession" button in the top right corner OR the "+" at the bottom of the "Related Accessions" section. You might have to hover to see the "+" at the bottom. 

### Agent Links

Maps to: ```<origination>``` and ```<controlaccess>```

Agents are person (```<persname>```), family (```<famname>```) or corporate (```<corpname>```) names that are associated with the collection as creators or subject headings (geographic names are entered as Subjects).

Need tips to create good agent links? There's <a href="https://github.com/UNC-Libraries/SCTS-Documentation/blob/main/Descriptive%20Elements.md#access-points">documentation</a> for that!


**Pro tip:** You can add more Agents by clicking the "Add Agent Link" button in the top right corner OR the "+" at the bottom of the "Agent Links" section. You might have to hover to see the "+" at the bottom.

- **Role:** Select "Creator" or "Subject."
  - Required to save record
  - Agents linked with the "creator" role will appear as the creator (```<origination>```).
  - Agents linked with the "subject" role will appear in the finding aid's subject headings ```<controlaccess>```).
  - If an agent is both the creator and a subject, link it twice, once with the "creator" role and once with the "subject" role.

<img width="530" height="135" alt="Picture9" src="https://github.com/user-attachments/assets/07aa6c9d-b80a-44ec-9d95-f1e6ed6d1539" />

 - **Agents:**
   - Required to save record
   - To link an existing agent record, you can either begin typing in the name and select from a list of autocomplete options presented by ArchivesSpace OR use the "Browse" option.
     - Autocomplete:
      <img width="528" height="152" alt="Picture10" src="https://github.com/user-attachments/assets/0d2fcb70-0852-42bc-9eb6-da117aa40635" />
   - If using the "Browse" option, search for and select the desired agent, and then click "Link."
     - Browse:
       
        <img width="530" height="146" alt="Picture11" src="https://github.com/user-attachments/assets/15a74c45-3e9f-48a9-bb70-07021f5c12e0" />
        <img width="578" height="326" alt="Picture12" src="https://github.com/user-attachments/assets/61cb8694-7e96-4f7a-9f76-ce95fe2d9563" />
        
   - Many agent records that were ingested into ArchivesSpace from EAD are not formatted correctly. Don’t worry...they’re fine as they are right now.
  
   - To create a new agent record, select "Create" and then select the type of agent record you wish to create (Person, Family, or Corporate Entity). A minimal agent record may be created by filling in only the required fields. The minimal record can be enhanced later by adding additional information in other fields and sub-records. For more details about creating new agent records, visit the <a href="https://archivesspace.atlassian.net/wiki/spaces/ArchivesSpaceUserManual/pages/1942945864/Agent+Record+Fields+from+3.0">Agent Record Fields</a> page in the ArchivesSpace Help Center.
     
     - Create:
       
    <img width="530" height="197" alt="Picture13" src="https://github.com/user-attachments/assets/b57903b4-99b6-4340-8ef4-e40f2ad1c9f0" />
    
     - If an agent is listed in <a href="https://authorities.loc.gov/">LCNAF</a>, paste the "LCCN Permalink" in the "Authority ID" field.

### Subjects

Subjects (```<subject>```, ```<geogname>```, ```<genreform>```) are the finding aid's topical subject headings. Adding subject headings is similar to adding agent links.

Need tips to create good subject headings? There's <a href="https://github.com/UNC-Libraries/SCTS-Documentation/blob/main/Descriptive%20Elements.md#access-points">documentation</a> for that!

**Pro tip:** You can add more Subjects by clicking the "Add Subject" button in the top right corner OR the "+" at the bottom of the "Subjects" section. You might have to hover to see the "+" at the bottom.

- **Subjects:**
  - Required to save record.
  - To link an existing subject record, you can either begin typing in the subject and select from a list of autocomplete options presented by ArchivesSpace OR use the "Browse" option.
  - If using the "Browse" option, search for and select the desired subject, and then click "Link."
  - Many subject records that were ingested into ArchivesSpace from EAD are probably not formatted correctly. Don’t worry...they’re fine as they are right now.
  - To create a new subject record, select "Create" and fill in the "Term" and "Type" fields. For more details about creating new subject records, visit the <a href="https://archivesspace.atlassian.net/wiki/spaces/ArchivesSpaceUserManual/pages/894664812/Subject+Record+Fields">Subject Record Fields</a> page in the ArchivesSpace Help Center.
    - If a subject heading is listed in <a href="https://authorities.loc.gov/">LCSH</a>, enter the "LCCN Permalink" in the "Authority ID" field.

To add personal, family, or corporate names as subject headings, see the "Agent Links" section above. For more details about creating new agent records, visit the <a href="https://archivesspace.atlassian.net/wiki/spaces/ArchivesSpaceUserManual/pages/1942945864/Agent+Record+Fields+from+3.0">Agent Record Fields</a> page in the ArchivesSpace Help Center.

### Notes
The 10 notes fields we use the most often appear automatically in all new resource records:
- Abstract
- Processing Information (includes the Identity Statement)
- Biographical and Historical Note
- Scope and Content
- Restrictions to Access
- Restrictions to Use (delete if not needed)
- Copyright Notice
- Preferred Citation
- Acquisitions Information
- Separated Materials (delete if not needed)

**Pro tip:** If you need to add another note that's not listed here, you can do so by clicking the "Add Note" button. \

<img width="624" height="496" alt="Picture14" src="https://github.com/user-attachments/assets/b034676f-124e-440b-9428-686fc7d0a5c5" />

You need to fill in each of these fields with collection-specific content (or delete if not needed). While in edit mode, click on the note you want to edit. The Persistent ID, Label, and Type fields will be pre-populated.

**Pro tip:** If you create a new note, you will need to fill in the "Label" field. Make sure to click on the "Publish?" box(es) or the note will not appear in Archy.


#### Abstract

> Required!

Fill in abstract information after the collection-level scope and content note is written!

Need tips on how to write a good abstract? There’s <a href="https://github.com/UNC-Libraries/SCTS-Documentation/blob/main/Descriptive%20Elements.md#abstract">documentation</a> for that!

<img width="729" height="175" alt="Picture15" src="https://github.com/user-attachments/assets/1150d84d-b4e6-4a9c-bbd3-0572c88f86b9" />

- **To create an abstract for a new resource record,** click on the automatically created **Abstract** note and either type directly into the "Content" field OR copy and paste from another file (Word doc, etc.).  Make sure to remove the boilerplate text!

- **To make a quick edit to an existing abstract,** simply make the change directly in the "Content" field.

- **To make major revisions (i.e., a more extensive rewrite that is not quick),** type revisions in another file (Word doc, etc.), and then copy and paste the new version into the "Content" field.


#### Processing Information

> Required!

<img width="695" height="232" alt="Picture16" src="https://github.com/user-attachments/assets/555a6eb6-5d70-4449-8b5d-eaef3f002021" />

**To create a processing information note for a new resource record,** click on the automatically created **Processing Information** note.

You will see the following boilerplate text:

```Processed by: [NAME], [MONTH YEAR]```
  
```Finding aid created by: [NAME], [MONTH YEAR]```
  
```In 2017, we began using "white" as an ethnic and racial identity for individual and families, in addition to "Black," "African American," "Jewish," and other familiar identity terms that we have used for decades in collection descriptions. We use this identity term so that whiteness is no longer the presumed default of the people represented in our collections. To determine identity, we rely on self-identification; other information supplied to the repository by collection creators or sources; public records, press accounts, and secondary sources; and contextual information in the collection materials. Omissions of ethnic and racial identities in finding aids created or updated after August 2017 are an indication of insufficient information to make an educated guess or an individual's preference for identity information to be excluded from description. When we have misidentified, please let us know at wilsonlibrary@unc.edu.```

Replace [NAME], [MONTH YEAR] with the correct information. 

- Examples: 
  - Processed by: Davia Webb, November 2024
  - Finding aid created by Laura Smith, February 2025
    
- **To make a quick edit to an existing processing information note,** simply make the change directly in the "Content" field. 

- **To make major revisions (i.e., a more extensive rewrite that is not quick),** type revisions in another file (Word doc, etc.), and then copy and paste the new version into the "Content" field.


#### Biographical and Historical Note

> Required!

Need tips on how to write a good biographical and historical note? There’s <a href="https://github.com/UNC-Libraries/SCTS-Documentation/blob/main/Descriptive%20Elements.md#biographicalhistorical-note">documentation</a> for that!

<img width="728" height="204" alt="Picture18" src="https://github.com/user-attachments/assets/a9ce2d56-3d68-4b94-a137-2cb9ea1f9af8" />

- **To create a biographical and historical note for a new resource record,** click on the automatically created Biographical and Historical note and either type directly into the “Content” field OR copy and paste from another file (Word doc, etc.). Make sure to remove the boilerplate text!

- **To make a quick edit to an existing biographical and historical note,** simply make the change directly in the “Content” field. 

- **To make major revisions (i.e., a more extensive rewrite that is not quick),** type revisions in another file (Word doc, etc.), and then copy and paste the new version into the “Content” field.


#### Scope and Content

> Required!

Need tips on how to write a good scope and content note? There’s <a href="https://github.com/UNC-Libraries/SCTS-Documentation/blob/main/Descriptive%20Elements.md#scope-and-content-note">documentation</a> for that!

<img width="728" height="204" alt="Picture19" src="https://github.com/user-attachments/assets/ecf80eaa-a65f-4c92-8950-9fd1b3cbfbb5" />

**To create a scope and content note for a new resource record,** click on the automatically created Scope and Content note and either type directly into the "Content" field OR copy and paste from another file (Word doc, etc.). Make sure to remove the boilerplate text!

- **To make a quick edit to an existing scope and content note,** simply make the change directly in the "Content" field. 

- **To make major revisions (i.e., a more extensive rewrite that is not quick),** type revisions in another file (Word doc, etc.), and then copy and paste the new version into the "Content" field.


#### Restrictions to Access

> Required!

<img width="626" height="258" alt="Picture20" src="https://github.com/user-attachments/assets/4c401423-05b3-46c3-8ec2-209e8719b737" />

- **To create a "Restrictions to Access" note for a new resource record,** click on the automatically created Restrictions to Access note and either type directly into the "Content" field OR copy and paste from another file (Word doc, etc.). Make sure to remove the boilerplate text!
  - *If there are no restrictions,* the correct statement is:  ```No restrictions. Open for research.```
  - *If restrictions apply,* refer to our <a href="https://github.com/UNC-Libraries/SCTS-Documentation/blob/main/Descriptive%20Elements.md#boilerplate-access-restriction-statements">Boilerplate Access Restriction Statements.</a>
     - *If the entire collection is not requestable*, also make sure that the "Requestable?" box is unchecked in the User Defined fields is unchecked. This ensures that the request buttons will not appear in Archy.

If applicable, select the appropriate access restriction type(s) from the “Local Access Restriction Type” box. To select more than one option or to deselect an option, hold down CTRL (Windows)/Command (Mac). The options are:

- 1 – Donor/university imposed access restriction 
- 2 – Repository imposed access restriction
- 3 – Restricted fragile
- 4 – Restricted in-process
- 5 – Other
  
You can also enter "Restriction Begin" and "Restriction End" dates.

- **To make a quick edit to an existing "Restrictions to Access" note,** simply make the change directly in the "Content" field. If applicable, change the "Restriction Begin" and "Restriction End" dates, as well as the access restriction type(s) from the "Local Access Restriction Type" box. To select more than one option or to deselect an option, hold down CTRL (Windows)/Command (Mac).

- **To make major revisions** (i.e., a more extensive rewrite that is not quick), type revisions in another file (Word doc, etc.), and then copy and paste the new version into the "Content" field. If applicable, change the "Restriction Begin" and "Restriction End" dates, as well as the access restriction type(s) from the "Local Access Restriction Type" box. To select more than one option or to deselect an option, hold down CTRL (Windows)/Command (Mac).

#### Restrictions to Use

> Delete if not needed.

<img width="624" height="324" alt="Picture21" src="https://github.com/user-attachments/assets/93204355-84a6-4f0b-a6f3-bc516674809a" />

To create a "Restrictions to Use" note for a new resource record, click on the automatically created Restrictions to Use note and either type directly into the "Content" field OR copy and paste from another file (Word doc, etc.). Make sure to remove the boilerplate text!

Add this field **ONLY** if there are use restrictions. Do not add a note saying that there are no restrictions. 

- **To make a quick edit to an existing “Restrictions to Use” note (i.e., correcting a typo),** simply make the change directly in the “Content” field. If applicable, change the "Restriction Begin" and "Restriction End" dates.

- **To make major revisions (i.e., a more extensive rewrite that is not quick),** type revisions in another file (Word doc, etc.), and then copy and paste the new version into the "Content" field. If applicable, change the "Restriction Begin" and "Restriction End" dates.

  
#### Copyright Notice

> Required for NCC, RBC, SFC, and SHC.
>
> Copyright does not apply to records in University Archives, since they are public records. However, copyright might still apply to some UARMS collections that aren't University Records, such as the <a href="https://finding-aids.lib.unc.edu/catalog/70204">Jean Freisleben Letters</a>.

This note contains the following boilerplate text:

```Copyright is retained by the authors of items in these papers, or their descendants, as stipulated by United States copyright law.```

Unless otherwise specified in the accession record, you do not need to do anything to this field.


#### Preferred Citation

> Required!

This note contains the following boilerplate text:

```[Identification of item], in the [collection name and number], Wilson Special Collections Library, University of North Carolina at Chapel Hill.```

You do not need to do anything to this field.


#### Acquisitions Information

> Required!


Need tips on how to fill out this field? There’s <a href="https://github.com/UNC-Libraries/SCTS-Documentation/blob/main/Descriptive%20Elements.md#acquisition">documentation</a> for that!

<img width="685" height="213" alt="Picture22" src="https://github.com/user-attachments/assets/dfda1670-8a54-46e4-be51-19de106e4168" />

- **To create acquisitions information for a new resource record,** click on the automatically created Acquisitions Information note and either type directly into the "Content" field OR copy and paste from another file (Word doc, etc.). Make sure to remove the boilerplate text!

- **To make a quick edit to an existing acquisitions information note,** simply make the change directly in the "Content" field. 

- **To make major revisions (i.e., a more extensive rewrite that is not quick),** type revisions in another file (Word doc, etc.), and then copy and paste the new version into the "Content" field.

#### Separated Materials

> Delete if note needed.

<img width="1310" height="579" alt="Picture24" src="https://github.com/user-attachments/assets/a1a84d25-a551-4ea1-bae8-89726c49351e" />

- **To create a “Separated Materials” note for a new resource record,** click on the automatically created Separated Materials note and either type directly into the "Items" field. Make sure to remove the boilerplate text! Click "Add Item" to add more than one item.

- **To make a quick edit to an existing separated materials note,** simply make the change directly in the "Item" or "Content" field.
  - This information might be stored in a "Content" field in finding aids created before August 2025.

### External Documents

Don’t worry about these fields, at least for right now. They can be used to link to information in other description management tools, such as donor files or processing plans. Maybe we’ll decide to use them in the future, but we’re not ready to experiment with it yet.

### Rights Statements

Don’t worry about these fields. We are not using them at this time.

### Metadata Rights Declarations

No need to worry about these fields. We are not using them at this time. Should we decide to start using them, the information will likely become part of the template that is automatically generated with new resource records.

### Instances

Instances refer to physical containers and digital objects.  **See <a href="https://github.com/UNC-Libraries/SCTS-Documentation/blob/main/Finding%20Aids%20in%20ArchivesSpace.md#adding-series-subseries-and-file-level-archival-objects">Adding Series, Subseries, and File Level Archival Objects (below) for how to add instances to resource records</a>.**

> *Please note the current workflow for adding instances to resource records differs from the workflow used during the ArchivesSpace implementation period (2020-2024). Please do not attempt to use the old workflow. Doing so will cause a lot of confusion in Archy and to our R&IS colleagues.*


### Deaccessions

These fields are used to record information about deaccessions, and should only be used by the Technical Services Archivist for Collection Management.

### Collection Management

Leave these fields blank. These fields are used to record processing information. Since we record this information on the accession records, this information does not need to be filled out here.

### Classifications

> Required!

We are using the Classifications field to record the curatorial unit. This field allows the curatorial units to appear as facets in Archy.

- **Maps to:** '''<repository>'''
- Required for indexing in Archy
- Select one (and only one) classification per resource record.
  -  The list of classifications tends to load very slowly. Never fear...it’s there. You’ll get to it eventually.
  -  Some existing resource records have two classifications: one indicating the curatorial unit and another indicating that it is an "Antebellum" collection. The "Antebellum" classification does not create a facet in Archy. *Do not* add the "Antebellum" classification to any additional records.
 
 <img width="1452" height="658" alt="Picture25" src="https://github.com/user-attachments/assets/8b708518-bb4b-48ec-870e-3a9dd564ce1d" />

In most cases, you will select SHC, SFC, UA, or NCCPA. However, there are a total of 10 options:

- **General Archival Collections (ULGAC)**
  - Examples:
    - Zbigniew Bujak Orange Revolution Photographs (60001)
    - Rebun Kayo Hiroshima Landslide Recovery Photographs, Videos, and Related Materials (60002)
  - You are unlikely to use this option.
    
- **North Carolina Central University Collections (NCCU)**
  - Examples:
    - James E. Shepard Papers (50001)
    - North Carolina Central University Faculty and Staff Photograph Records (50007)
  - These materials are owned by and are housed at NCCU. You are unlikely to use this option.
 
- **North Carolina Collection (NCC)**
  - Examples:
    - Wolfe Family Papers (70003)
    - North Carolina City, County, and Regional Ephemera Collection (70023)
  - To be used for NCC collections that are not NCCPA.

- **North Carolina Collection Photographic Archives (NCCPA)**
  - Examples:
    - North Carolina County Photographic Collection (P0001)
    - Virginia Omega Collier Photograph Album (70146)
      
- **Rare Book Collection (RBC)**
  - Examples:
    - American and English Playbills (70027)
    - A. P. Watt Records (11036)
      
- **Southern Folklife Collection (SFC)**
  - Examples:
    - William R. Ferris Collection (20367)
    - Roland L. Freeman Photograph Collection (70147)
   
- **University Archives (UA)**
  - Examples:
    - Board of Trustees of the University of North Carolina Records (40001)
    - Asian American Center of the University of North Carolina at Chapel Hill Records (70102)

- **North Carolina Central University/Southern Historical Collection (NCC/SHC)**
  - Examples:
    - Floyd B. McKissick Papers (04930)
    - Alan McSurely Papers (04928)
  - These materials are jointly held collections between North Carolina Central University and the Southern Historical Collection. You are unlikely to use this option.

- **Southern Historical Collection (SHC)**
  - Examples:
    - Hayes Collection (00324)
    - G. K. Butterfield Papers (70106)
   
- **Antebellum (Antebellum)**
  - Used for internal purposes only to track collections previously identified as having "antebellum" or "slavery-era" content.
  - Do not assign this classification to any collection unless specifically instructed to do so by Jackie Dean.


### User Defined

These fields are used to record additional information not accounted for in other fields. They are for internal purposes only and will not display in the finding aid.
At this time, we are using the following User Defined fields for resource records. More fields might be added in the future:

 - **Contains harmful content?:** Check this box if a collection contains materials with harmful content.
   - Examples:
    - Photographs of lynchings
    - Letters that contain hate speech
 - **Requestable?**
   - Check this box if materials should be requestable in Archy.
 - **Description of harmful content:** Use this box to describe the materials with harmful content. 
   - Examples:
     - Image folder 7 contains photographs of lynchings.
     - Folder 10 contains letters that contain racist language.


# Adding Series, Subseries, and File Level Archival Objects

Now it's time to add your series/subseries/files/etc. to the resource record. There are two ways to create new archival objects in ArchivesSpace: manually using "Rapid Data Entry (RDE)," and via the "Load via Spreadsheet" option:

- "Rapid Data Entry (RDE)" is a convenient way to enter information if you only have one series AND have time to enter all your information in one sitting (you could still use it if you have more than that, but the word "Rapid" is in there for a reason.)
  - You can also enter components manually without using the Rapid Data Entry option, but I only recommend doing so if you’re making minor edits to existing components (see documentation about revisions below). Otherwise, it’s really not worth the hassle.
- "Load via Spreadsheet" is a good option if you have more than one series, have multiple subseries, OR don’t have time to do all your data entry in one sitting.

**Pro tip:** IMO the spreadsheet is easier to use regardless, but feel free to experiment to determine what works best for you.

## Rapid Data Entry

> <a href="https://archivesspace.atlassian.net/wiki/spaces/ArchivesSpaceUserManual/pages/893976919/Using+the+Rapid+Data+Entry+RDE+Tool+to+Create+Multiple+Resource+Component+Records">ArchivesSpace Help Center</a>

First, you need to create a new series:

 - In edit mode, click on the collection title at the top of the tree structure and click on "Add child."

<img width="626" height="67" alt="Picture26" src="https://github.com/user-attachments/assets/f37550d2-e0ab-47ae-b7a2-734215368963" />

- Fill out the following fields:
  - **Title:** The series title
  - **Level of Description:** Select “Series” from the drop menu
  - **Publish?"**: Make sure this box is checked
  - **Dates:** Follow the instructions under <a href="https://github.com/UNC-Libraries/SCTS-Documentation/blob/main/Finding%20Aids%20in%20ArchivesSpace.md#dates">Collection-level Fields and Notes</a> (above)
  - **Extents:** Follow the instructions under <a href="https://github.com/UNC-Libraries/SCTS-Documentation/blob/main/Finding%20Aids%20in%20ArchivesSpace.md#extents">Collection-level Fields and Notes</a> (above)
  - Notes: Create a scopecontent note. You will need to create it yourself; it will not automatically appear as it does on the collection-level record.
    - Make sure the "Publish?" checkbox is checked. 
- Click “Save.”

In edit mode, click on your newly created series and select the "Rapid Data Entry" option.

The following screen will appear:

<img width="624" height="230" alt="Picture27" src="https://github.com/user-attachments/assets/65964309-2e3a-4599-9b21-1b5a75d4292d" />

The notes in the gray box are helpful!

<img width="624" height="229" alt="Picture28" src="https://github.com/user-attachments/assets/47271f65-b6f7-46b3-a1b4-a8a78c9c8a61" />

Enter desired data. The "Level of Description" element (in this case, probably "File") and either "Title" or one of the "Dates" sub-record elements is required. You can add other information, such as "Extent," as appropriate. Always make sure to check the "Publish?" checkbox.

Make sure to add a Top Container and at least one Child Type and Child Indicator so that we’ll be able to page the materials later. [Note that you cannot link to locations to top containers from the Rapid Data Entry screen. You will link locations to the top containers via <a href="https://github.com/UNC-Libraries/SCTS-Documentation/blob/main/Labelling%20and%20Putting%20Stuff%20Away.md#linking-to-locations-in-archivesspace">Manage Top Containers</a> after you are done adding archival objects.]

- Example: Let’s say we are adding Image Folder 1, which is in Image Box 1 to collection 90001. You will fill out the fields like this:
  - **Instance Type:** Mixed materials (this is the only "Instance Type" we are using.)
  - **Top Container:** If Image Box IB-90001/1 already exists, begin typing it into the Top Container field. The box should appear as an option that you can select. If it does not already exist, click on “Create,” enter "Image Box" into the "Container Type" field and "IB-90001/1" into the "Indicator" field. You can scan the barcode at this time, but it’s not necessary to do so – it's easy to go back and do that later.
  - **Child Type:** Image Folder
  - **Child Indicator:** PF-90001/1
  - You can also enter **grandchild** information if needed

<img width="585" height="228" alt="Picture29" src="https://github.com/user-attachments/assets/5c5dd44d-1319-4f4b-8af3-19e46e571e47" />

Add as many rows as needed to record additional archival objects, then click “Save” when you are done.

The new archival objects are now part of the record:

<img width="701" height="156" alt="Picture30" src="https://github.com/user-attachments/assets/129f2a42-eb98-4b66-b9a1-cde422e92692" />

## Load via Spreadsheet

> <a href="https://archivesspace.atlassian.net/wiki/spaces/ArchivesSpaceUserManual/pages/1173913646/Importing+Archival+Objects+from+Excel+or+CSV+File+from+v2.8.1-3.3.)">ArchivesSpace Help Center</a>

Use the spreadsheet located in Teams: Wilson SCTS-Archival > ArchivesSpace > Files > FREEZE > bulk_import_template_2024.xlsx. Make sure to save the copy you're editing to your desktop (or "save as" with a different filename) to make sure someone else doesn"t overwrite your work! 
> This file will probably move to LOUIS in the near future. These instructions will change when/if that happens.

You can also download a new spreadsheet from the resource record by clicking on the gear wheel, selecting "Bulk Import Templates," and then "Bulk Import AO XLSX."

There’s A LOT of fields, but don’t panic…you can ignore most of them. The spreadsheet is trying to account for every field that you can possibly use. 
> Just as we didn't use most of these fields when we were encoding EAD finding aids, we're not going to use most of them now, either.

<img width="576" height="300" alt="Picture31" src="https://github.com/user-attachments/assets/0eacb59d-e3e0-4b18-a5ae-b30faa3717ae" />

Here’s the fields you are most likely to use (note that many of the fields have drop menus). Some fields, such as "EADID" and "Title," will be used for every archival object that you enter. Other fields, such as the extent fields and the note fields, should be filled out for series-level archival objects, but can also be added to lower-level archival objects as applicable. 

- **Basic Information (Columns C-M):**
  - **EADID (Column C, required):** This should be the same as the collection number and should match the “EAD ID” field in the resource record.
  - **Title (Column F, required):** The title of the archival object. This is typically and folder title or box title. Add the date, too, even though this will also be recorded in the date field.
    - **Maps to:**  ```<unittitle>``` 
  - **Hierarchical Relationship (Column H, required):** In most cases, series will have a hierarchical relationship of “1,” while folder or box titles will have a hierarchical relationship of “2.” If you add a second series, it will also have a hierarchical relationship of “1.”
    - This is like nesting ```<c0x>```s in EAD.
  - **Description Level (Column I, required):** Select appropriate level from the drop list ("Series," "File," etc.). 
  - **Publish? (Column K):** In most cases, you will set to "True."
  - **Restrictions Apply? (Column L):** Select if applicable.

- **Dates (Columns V-AG):**
  - Columns W-X are for normalized dates. Column Z is for inclusive dates.
  - **Date(1) label (Column V, required if entering a date):** Should almost always be "creation."
  - **Date(1) Begin (Column W):** Beginning of the date range
    - Normalized date
  - **Date(1) end (Column X):** End of the date range
    - Normalized date
  - **Date(1) Type (Column Y, required if entering a date):** Select from drop menu.  Will usually be "inclusive."
  - **Date (1) expression (Column Z, required if entering a date):** Enter date expression
    - Inclusive date
    - Examples: 1980-1981; 1950s-2000s; circa 1945-1982

- **Extent Information (Columns AH-AS):**
  - **Extent Number (Column AI)**
  - **Extent Type (Column AJ)**

- **Container information (Columns AT-BI):**
  - **Container Instance Type (Column AT):** Should always be ```mixed_materials```
    - ```mixed_materials```, *not* "mixed materials" or "Mixed_Materials," or other variations
  - Top Container type (Column AU): Most likely "Document Case," "Record Carton," "Image Box," or "Oversize Box."
    - Make sure to capitalize the "D" and "C" in “Document Case” and the "R" and "C" in "Record Carton."
  - **Top Container Indicator (Column AV):** The container number.
  - **Barcode (Column AW)**: DON'T enter this information here. It tends to cause problems. The stacks manager (Margaret) will enter it later (see <a href="https://github.com/UNC-Libraries/SCTS-Documentation/blob/main/Labelling%20and%20Putting%20Stuff%20Away.md#linking-locations-in-archivesspace">Linking to Locations in ArchivesSpace</a>)
  - **Child type (Column AX):** Subcontainer type, if used. Most likely “folder,” “Image Folder,” or “Oversize Paper.”
    - In most cases, you will capitalize the first letter of each word ("Image Folder," "Oversize Paper," etc.)
    - There are two exceptions: ```folder``` and ```box``` (and you're probably not going to use "box.")
  - **Child indicator (Column AY):** The subcontainer (folder, image folder, etc.) number.
  - **Grandchild type (Column AZ):** The sub-subcontainer type, if used. Most likely "Image," or "Oversize Paper."
  - **Grandchild indicator (Column BA):** The sub-subcontainer (image, oversize paper, etc.) number.

- **Notes (Columns ED-GE):**
  - **Access Restrictions (Column EG):** Add as applicable.
  - **Publish Access Restrictions (Column EH):** To be used if filling out Column EG. In most cases, you will set to "True."
  - **Acquisition Information (Column EM):** Add as applicable.
  - **Publish Acquisition Information? (Column EN):** To be used if filling out Column EM. In most cases, you will set to "True."
  - **Scope and Contents (Column FW):** Add as applicable.
  - **Publish Scope and contents? (Column FX):** To be used if filling out Column FW. In most cases, you will set to "True."
  - **Use Restrictions (Column GC):** Add as applicable.
  - **Publish Use Restrictions? (Column GD):** To be used if filling out Column GC. In most cases, you will set to "True."
 
Again, there’s A LOT more fields that you can use if needed (although most of the time you probably won’t).

Once you’re done filling out the spreadsheet, navigate to the resource record you’re updating, and select where the new archival objects should be located within the existing tree structure.

- If you are adding a new series, click on the collection-level archival object at the top of the tree structure.
- If you are adding archival objects to an existing series, click on the series within the tree structure.

**Pro tip:** If you accidentally add your new archival objects to the wrong place, you can either delete them and re-import them, or use the <a href="https://archivesspace.atlassian.net/wiki/spaces/ArchivesSpaceUserManual/pages/894140803/Reordering+Components+in+Resource+Records+from+version+3.5.0">Enable Reorder Mode</a> feature to move/rearrange. 

While in edit mode, select the “Load via Spreadsheet” option.

<img width="610" height="109" alt="Picture32" src="https://github.com/user-attachments/assets/f90bc9a9-1330-4cf5-bbc5-4435b04a38ed" />

You will be prompted to select a file to import. Select your spreadsheet using the green "Select File" (you will need to save and close it first). Then click on the "Import from SpreadSheet" button (I don’t know why it’s spelled "SpreadSheet" and I wish someone would change it).

<img width="609" height="168" alt="Picture33" src="https://github.com/user-attachments/assets/59492504-eda2-4d2f-bf91-823d76be2f56" />

You will see a Background Job status screen that will go through several job status steps. If the spreadsheet successfully imports, you should see a screen that looks something like this:

<img width="608" height="307" alt="Picture34" src="https://github.com/user-attachments/assets/dc36a988-05fe-411b-9cd0-77fee6a21666" />

Your new archival objects are now part of the resource record. Note that the top containers now appear, but they will not have locations linked to them. You still need to do that manually via <a href="https://github.com/UNC-Libraries/SCTS-Documentation/blob/main/Labelling%20and%20Putting%20Stuff%20Away.md#linking-locations-in-archivesspace">Manage Top Containers</a>.

<img width="609" height="287" alt="Picture35" src="https://github.com/user-attachments/assets/929ae933-a5aa-478f-a8ea-b7be31fee996" />

If the import fails, and you can't figure out why it failed, contact Dawne and we'll try to figure it out together.

# Revising Series, Subseries, and File Level Archival Objects

> As the title suggests, this section is about revising **existing** archival objects. If you are adding new archival objects, please follow the instructions in the <a href="https://github.com/UNC-Libraries/SCTS-Documentation/blob/main/Finding%20Aids%20in%20ArchivesSpace.md#adding-series-subseries-and-file-level-archival-objects">Adding New Series, Subseries, and File Level Archival Objects</a> section above. This includes adding new archival objects to an existing series or subseries. Basically, if it’s an archival object that’s not already in ArchivesSpace, follow the instructions in the previous section. If you are revising an archival object that’s already in ArchivesSpace, follow the instructions below.
> 
> Unless the content is being removed from the collection, DO NOT DELETE existing archival objects if there is an associated digital object. Doing so will break the link to the digital object, meaning it will no longer appear in the finding aid. [All is not lost if you delete something that shouldn’t have been deleted, but it’s best to avoid doing so.]

**If you are revising an existing resource record, change the "Finding Aid Status" field to "Under Revision." Make sure to change it to "Completed" once you are done.**

There are two ways to revise existing archival objects in ArchivesSpace: manually, and via the "Bulk Update Spreadsheet" plug-in option:

- Manual data entry is ideal for making quick, easy edits that don’t require the spreadsheet option mentioned below. 
- This bulk update spreadsheet is a great feature for edits that aren’t as quick and easy, such as bulk editing existing date ranges and other folder titles.
  - Did you make the same typo on every archival component in a series? This option is for you!

> Technically speaking, you can also use the "Load via Spreadsheet" option detailed above to edit existing archival objects, BUT it will create another copy, meaning you will need to delete the older, unedited archival object. DO NOT DO THIS without good reason, as doing so will break the links to any associated digital objects, top containers, etc. (A large-scale reprocessing project resulting in enhanced description and a completely different arrangement is probably a good reason. A small-scale rearragement that can be accomplished by using the <a href="https://archivesspace.atlassian.net/wiki/spaces/ArchivesSpaceUserManual/pages/894140803/Reordering+Components+in+Resource+Records+from+version+3.5.0">Enable Reorder Mode</a> feature is not). 

## Manual Data Entry

This option is ideal for making quick, easy edits that don't require the spreadsheet options mentioned below. Need to fix a typo or edit a date range? Then this option is for you! In edit mode, simply click on the archival object that needs editing, make your edit, and click "Save."

## Bulk Archival Object Updater

You can use the Bulk Archival Object Spreadsheet to edit existing archival objects. This is a great feature for updating existing date ranges, container information, etc. You cannot use it to create new archival objects.
From the resource record, click on "More," and then "Bulk Archival Object Spreadsheet."

<img width="568" height="214" alt="Picture36" src="https://github.com/user-attachments/assets/13332753-5788-4d32-8dbd-8514e60aa2ba" />

You will now see a screen with all of the resource's archival objects. Select the archival objects you wish to edit, then click "Download Spreadsheet" (not pictured below, in the bottom left corner of your screen). 

<img width="568" height="196" alt="Picture37" src="https://github.com/user-attachments/assets/9b57fa57-44e2-45a3-a012-c0a95b93abf2" />

Save the file to your computer (**DO NOT** change the file name) and then open it (you can then click the "Cancel" button next to the "Download Spreadsheet" button to return to the resource record). The file looks like a scaled down version of the "Load via Spreadsheet" template. Make your edits and save.

<img width="626" height="215" alt="Picture38" src="https://github.com/user-attachments/assets/2f5f91b5-e880-4b22-9a10-72c0ed8da218" />

To upload the edited data, select Create > Background Job > Bulk Archival Object Updater.

<img width="578" height="240" alt="Picture39" src="https://github.com/user-attachments/assets/674b8915-b47e-4a6f-8d2a-086203ecd992" />

Select your spreadsheet file, and then click "Start Job."

<img width="578" height="140" alt="Picture40" src="https://github.com/user-attachments/assets/9920505e-05dc-4d9c-a555-52a50a0509cf" />

You will see a Background Job status screen that will go through several job status steps. If the spreadsheet successfully imports, you should see a screen that looks something like this:

<img width="614" height="238" alt="Picture41" src="https://github.com/user-attachments/assets/8384a7d8-6999-4d92-b45e-5a0ea447154e" />

Your archival objects have now been edited. If the import fails, and you can’t figure out why it failed, contact Dawne and we’ll try to figure it out together!

# Finding Aid Publication Workflow

**In pipette-qa**

- Use pipette-qa to preview changes before submitting a ticket for them to go live.
- Login to https://finding-aids-qa.lib.unc.edu/admin using your Onyen.
- Select the finding aid you’d like to index from the list on the "Collections" screen. If your finding aid does not appear:
  - Click on the green "Pull in Latest Aspace Updates" button.
  - If that doesn't work, Make sure that the resource record has a classification linked to it and the "Publish?" checkbox is checked.
  - If that doesn’t work, let Dawne know.
- Click on the blue “Index selected collections” button. A dashboard will appear showing the status of three tasks: downloading the XML from ArchivesSpace, indexing in Archy, and creating the PDF. Once these tasks are complete, you can view the finding aid at https://finding-aids-qa.lib.unc.edu/.
  - NB: The status board will stop updating after 5 minutes, although usually that is more than enough time to index your updates.
  - DO NOT click on the blue "Display all Resources" button. Nothing bad will happen, but it will take a very long time for that task to complete.
- Repeat these steps until you are ready for the finding aid to go live.

**In ArchivesSpace**

- Make sure that all fields that should be published are in fact published. If there are fields that shouldn’t be published, make sure the “Publish?” box is unchecked.
- Make sure that you have linked a classification.
- Change the "Finding Aid Status" field to "Completed."
- Remember to save your work!  

**In Teams**

- Submit a "Blue Sheet" or "Merge Request" ticket (form is pinned to the top of the Wilson TS-Archival General channel). Laura Smith will make the changes go live.
  - Students who are not assigned to TS-Archival might not have access to this Teams channel. If this scenario applies to you, work with Dawne to submit the ticket. 

# Finding Aid Checklist

See <a href="https://github.com/UNC-Libraries/SCTS-Documentation/blob/main/Finding%20Aid%20Checklist.md">Finding Aid Checklist</a>


