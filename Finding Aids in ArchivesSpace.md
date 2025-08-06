Created by Dawne Lucas in August 2025

# Creating Finding Aids in ArchivesSpace

# Overview

 - [Introduction: ArchivesSpace, ArcLight (Archy), and Pipette](#introduction)
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
   - [Adding Series, Subseries, and File Level Archival Objects](#adding-series)
   - [Revising Series, Subseries, and File Level Archival Objects](#revising-series)
   - [Finding Aid Publication Workflow](#finding-aid-publication-workflow)
   - [Finding Aid Checklist](#finding-aid-checklist)
  
   ***

   # Introduction: ArchivesSpace, ArcLight (Archy), and Pipette

These are instructions for creating finding aids using ArchivesSpace, Pipette, and ArcLight (Archy).

Here’s the very tl;dr summary of the difference between the three:

 - **ArchivesSpace:** Staff-only interface used to create finding aids.
 - **ArcLight (Archy):** Public-facing interface used to display finding aids. 
   - UNC's version of ArcLight was named "Archy" (ArcLight at UNC-Chapel Hill) by Library Software Applications Developer Dean Farrell. "Archy" is UNC-specific, and the name is not used by other institutions using ArcLight.
 - **Pipette:** Staff-only interface used to preview and publish finding aids in ArcLight. 
   - NB: Content published to ArcLight is tracked via Git/Sourcetree, but TS-Archival does not interact with it. 
   - This is a UNC-specific application.
   - 
Remember: these are merely new tools for creating and displaying finding aids and do not replace our best practices for archival description:

 - <a href="https://github.com/UNC-Libraries/SCTS-Documentation/blob/main/Descriptive%20Elements.md">Descriptive Elements</a>
 - <a href="https://github.com/UNC-Libraries/SCTS-Documentation/blob/main/Style%20Guide.md">Style Guide</a>

# ArchivesSpace Terminology

ArchivesSpace comes with its own jargon that might be new to you. Here are some terms that you should learn to love:

 - **Archival object:** Unit of archival description, such as a folder title.
   - Archival objects map to components (<c0x>) in EAD. 
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
 

   
