Created by Dawne Lucas in August 2025 (in progress)

# Creating Finding Aids in ArchivesSpace at UNC-Chapel Hill

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
   - [Revising Series, Subseries, and File Level Archival Objects](#revising-series-subseries-and-file-level-archival-objects)
   - [Finding Aid Publication Workflow](#finding-aid-publication-workflow)
   - [Finding Aid Checklist](#finding-aid-checklist)
  
   ***
   
# Introduction: ArchivesSpace, ArcLight (Archy), and Pipette

These are instructions for creating finding aids using ArchivesSpace, Pipette, and ArcLight (Archy) at the Wilson Special Collections Library at UNC-Chapel Hill. This documentation is supplemental to the documentation provided by ArchivesSpace, and has been adapted for use at the Wilson Special Collections Library.

Here’s the very tl;dr summary of the difference between the three:

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

### Extents

### Finding Aid Data

### Revision Statements

### Related Accessions

### Agent Links

### Subjects

### Notes

#### Abstract

#### Processing Information

#### Biographical and Historical Note

#### Scope and Content

#### Restrictions to Access

#### Restrictions to Use

#### Copyright Notice

#### Preferred Citation

<span style="color:red">*Required!*</span>

This note contains the following boilerplate text:

```[Identification of item], in the [collection name and number], Wilson Special Collections Library, University of North Carolina at Chapel Hill.```

You do not need to do anything to this field.


#### Acquisitions Information

#### Separated Materials

### External Documents

Don’t worry about these fields, at least for right now. They can be used to link to information in other description management tools, such as donor files or processing plans. Maybe we’ll decide to use them in the future, but we’re not ready to experiment with it yet.

### Rights Statements

Don’t worry about these fields. We are not using them at this time.

### Metadata Rights Declarations

No need to worry about these fields. We are not using them at this time. Should we decide to start using them, the information will likely become part of the template that is automatically generated with new resource records.

### Instances

Instances refer to physical containers and digital objects.  **See Adding Series, Subseries, and File Level Archival Objects (below) for how to add instances to resource records.**

> *Please note the current workflow for adding instances to resource records differs from the workflow used during the ArchivesSpace implementation period (2020-2024). Please do not attempt to use the old workflow. Doing so will cause a lot of confusion in Archy and to our R&IS colleagues.*


### Deaccessions

These fields are used to record information about deaccessions, and should only be used by the Technical Services Archivist for Collection Management.

### Collection Management

Leave these fields blank. These fields are used to record processing information. Since we record this information on the accession records, this information does not need to be filled out here.

### Classifications

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

# Revising Series, Subseries, and File Level Archival Objects

# Finding Aid Publication Workflow

# Finding Aid Checklist


