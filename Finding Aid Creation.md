# Overview

- [Collection Level Records](#collection-level-records)
- [Adding container lists to existing collection level records](#adding-container-lists-to-existing-collection-level-records)
- [Creating collection level records](#creating-collection-level-records)

***

# Collection Level Records

**Check with Laura Smith**

Collection level records for unprocessed materials will contain the elements prescribed by DACS for a single-level minimum record. These elements are the following:  

- Reference Code Element (2.1)

- Name and Location of Repository Element (2.2)

- Abstract*

- Title Element (2.3)

- Date Element (2.3)

- Extent Element (2.5):

```
<physdesc label="Extent"> <extent encodinganalog="300">Add extent here. It can be rough.</extent> </physdesc>
```

- Name of Creator(s) Element (2.6) (if known) : we will check our catalog and LC authorities

- Conditions Governing Access Element (4.1): This collection is not available for immediate or same day access. Please contact Research and Instructional Service staff at wilsonlibrary@unc.edu to discuss options for consulting this collection.  

> Revise attribute: `<accessrestrict type="unprocessed">`

- Languages and Scripts of the Material Element (4.5)

- Processing info: This summary description was created in Month Year to provide information about unprocessed materials in Wilson Special Collections Library. 

***

If present in the AT record:

- Scope and Content Element (3.1)

*Bio note

> Note: Finding aids and catalog records for unprocessed materials will not contain subject headings. We'll attempt to write names in the authorized format but will not have these vetted by TS Biblio.  


[EAD Coding Examples](https://intranet.lib.unc.edu/wikis/msspace/index.php/Coding_examples)


# Adding container lists to existing collection level records

1. In Sourcetree, make sure you're on the right branch. 

2. Open Oxygen. Open the xml file you need to edit from the finding aid repository 

   (Users\username\Documents\finding-aids). File name = collection number. 

3. Make sure the url in the header (line 3) is **https**, and not **http**. 

4. Remove type="unprocessed" from the accessrestrict tag. 

   - `<accessrestrict type="unprocessed">` becomes just `<accessrestrict>`
   
   - Unless there are restrictions on the collection, remove the restriction note within the `<p>` tags and replace with `<p>No restrictions. Open for research.</p>`
   
5. Add identity to the abstract if you can make a reasonable assumption. 
   
6. Remove the comment out tags (`<!-- -->`) from the userestrict. Should read `<p>No usage restrictions.</p>` unless restrictions apply. 
   
7. Remove the comment out tags from acqinfo and include acquisitions information and accession number within the `<p>` tags. 
   
   Example:
      
   ```
   <acqinfo encodinganalog="541"> 

   <head>Acquisitions Information</head> 

   <p>Received from John Smith in April 2019 (Acc. 123456).</p> 

   </acqinfo> 
   ```

8. In `<processinfo>`, remove the summary description (This summary description was created...), and replace with `<p>Processed by [your name], [month year]`

   - Add `<p></p>` tags, and put the identity statement between them. 
   
     ```
     <p>Since August 2017, we have added ethnic identities for individuals and families represented in collections. To determine ethnic identity, we rely on self-identification; other information supplied to the repository by collection creators or sources; public records, press accounts, and secondary sources; and contextual information in the collection materials. Omissions of ethnic identities in finding aids created or updated after August 2017 are an indication of insufficient information to make an educated guess or an individual’s preference for ethnicity to be excluded from description. When we have misidentified, please let us know at wilsonlibrary@email.unc.edu.</p>
     ``` 

9. Add container list under `<head>Detailed Description of the Collection</head>`

   - Remove the coment out tags.
   
   - Remove "Enter Description Information Here" and replace with container list.
   
   - Start with `<c01>` tags.
   
     ```
     <c01 level="collection"> 

          <did><unittitle>[collection title, collection dates]</unittitle></did> 

     </c01> 
     ```

   - Add `<c02>` tags for each container listing, between `</did>` and `</c01>`
   
     ```
     <c01 level="collection"> 

          <did><unittitle>[collection title, collection dates]</unittitle></did> 

          <c02><did><container type="[container type]">[Container number]</container><unittitle>[Box/folder title]</unittitle></did></c02> 

     </c01> 
     ```

   - Refer to container type list under the EAD tab of the notebook for valid container types and how to write container numbers. 

   - Clean up container title capitalization, etc. 

10. Optional tags:

    - `<scopecontent><p>[Scope/content note]</p></scopecontent>`
   
      - Use for notes about content of the container that's not in the title. Goes between `</did>` and `</c02>`
      
    - `<accessrestrict><p>[Restriction note]</p></accessrestrict>`
    
      - Use for restrictions on containers. Goes between `</did>` and `</c02>`
      
    - For titles that need to be in italics, use `<title render="italic">[Title]</title>`
    
    - Copy/paste any diacritics. 
    
11. Transform the xml file to check your work. In Oxygen, click on the wrench with the red triangle, select your transformation scenario, and apply associated. The transformation should load in your default browser. 

12. Save changes in Oxygen.  

13. On your branch in Sourcetree, you should see "uncomitted changes" at the top of the log/history. Click on File Status and stage the file to commit. In the comment field, add a comment with [Collection number]: [brief description of changes made], then click commit. Keep the "push changes immediately" box checked. If Sourcetree tells you there are changes to push after you've committed, click the push arrow (but make sure you're on your branch first!)  

14. Fill out a blue sheet and give to Laura Smith when you're done.  


# Creating collection level records

1. Make sure you're on your branch in sourcetree. 

2. Login to unctechservices@gmail.com and navigate to the backlog folder. Find a backlog ticket not marked as "done." 

3. Open the backlog tracking spreadsheet, located in departmental document in sharepoint. Add the collection information into the tracking sheet. 

4. In oxygen, open the flasher template for the right Collection (SFC, SHC, UA). Templates are located here: G:\wilson\ts\archival\CLR_templates 

5. With the template open in oxygen, save the file in the git repo as the collection number. Save as-->navigate to C:\Users\[username]\Documents\finding-aids\[Collection]-->save as [collection number].xml.  

   For example, if you're working on a SHC collection, you should have the file saved as the collection number (ex. 05678.xml) under C:\Users\[username]\Documents\finding-aids\SHC. When saved here, "uncommitted changes" should show up at the top of your log/history on your branch in sourcetree. 

6. Follow the find-and-replace flasher directions at the top of the xml file with the information provided in the ticket. When done, delete flasher directions. 

7. Fill out the creator, extent, and abstract. Add a bio/hist and scope/content if included in the ticket. 

   - Creator could use `<persname>`, `<corpname>`, or `<famname>` depending on type of creator. 
   
   - You may only be given one form of extent (item count or linear feet). If so, just include it in the correct tags and comment out the other field. 
   
   - Please keep "Acquired as part of..." sentence at the end of the abstract. 
   
   - If including a bioghist note, change the header to either Biographical or Historical depending on the type of note. E.g.
   
     ```
     <head>Biographical/Historical Note</head> becomes <head>Biographical Note</head>
     ```
     
8. Transform the file and check everything over. 

9. Commit/push your changes on your branch in sourcetree. 

10. Label the email ticket as "Done." 

11. Mark x under "collection level finding aid" for the collection in the backlog tracking spreadsheet.  
