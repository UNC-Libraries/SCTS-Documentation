# Overview

- Extent
- Mold
- Literary papers
- Restricted materials
- XML to TXT script
- Excel formulas/tips
- Arrangement
- Drop in numbering for digitization requests


***

# Extent

Document case (or Hollinger box): about 400 items / .5 linear feet 

Records carton (or Paige box): about 800 items in legal folders, about 1200 items in letter folders / 1.5 linear feet 

(items separated i.e. photographs, oversize volumes, etc., are included in item counts, but not in linear feet) 


# Mold: A photo gallery

### Examples of mold 

Mold on a page:

![mold on a page](https://user-images.githubusercontent.com/58087302/80126423-104c9e00-8561-11ea-8791-aac2432bec35.jpeg "mold on a page")

Mold extreme close-up:

![mold close up](https://user-images.githubusercontent.com/58087302/80126531-3d00b580-8561-11ea-90c3-5fc00ae9107e.jpeg "mold close up")

Mold and water damage:

![mold and water damage](https://user-images.githubusercontent.com/58087302/80126767-71747180-8561-11ea-804c-3b48ce315767.jpeg "mold and water damage")

Hardcore mold and water damage:

![hardcore mold and water damage](https://user-images.githubusercontent.com/58087302/80126869-8e10a980-8561-11ea-9ed8-c97f225b10e1.jpeg "hardcore mold and water damage")

Color bleeding, water damage, and mold:

![color bleeding, water damage, and mold](https://user-images.githubusercontent.com/58087302/80126986-ada7d200-8561-11ea-87dd-c7b078d5a93e.jpeg "color bleeding, water damage, and mold")

Mold on a book cover:

![bold on book cover](https://user-images.githubusercontent.com/58087302/80127355-332b8200-8562-11ea-8bbc-eca2884d79fc.jpeg "mold on book cover")


# Literary papers

### Life Cycle of a Publication

![idea to book figure](https://user-images.githubusercontent.com/58087302/80127592-8a315700-8562-11ea-98ab-fdd2623d2a27.jpeg)


# Restricted materials

Restricted materials should be isolated in their own folders and labeled "RESTRICTED." Restricted folders do not necessarily need to be isolated in their own boxes if the restriction does not prohibit all access by researchers. Closed folders are always isolated in their own boxes and filed at the end of the collection. 


# XML to TXT script

Use the Saxon script to convert finding aid XML files to TXT files. This is an easy way to get finding aid data into a spreadsheet friendly format. Please note this script only exports limited fields from the XML file. At this time, nothing below the item title (i.e. ```<genreform>```, ```<scopecontent>```) can be exported through this script). The Saxon script exports the following fields from the XML file: 

- Collection Name 
- Collection Number 
- Location in Collection 
- Object (contains hook_id and item title) 
- Preferred Citation 
- Container Type 
- hook_id 
- Usage rights

### Instructions

**1.** Copy the “saxon” folder from the Tech Services Louis page to your desktop (Departmental Documents>TS_Archival>saxon): https://adminliveunc.sharepoint.com/:f:/r/sites/lib/departments/wts/Shared%20Documents/TS_Archival/saxon?csf=1&e=3hE3Ul 

**2.** Make a copy of the xml file for the finding aid. Put the copy in the saxon folder on your desktop. 

**3.** Open command line and type in the following commands 

   ```
   cd desktop/saxon;  

   java -jar saxon9he.jar -o :[insert name of output text file] 
   [insert name of finding aid file] ead2cdm_automate.xsl 
   ```
   
**Example command for 20367 finding aid:**

   ```
   Example command for 20367 finding aid:  

   java -jar saxon9he.jar -o:20367.txt 20367.xml ead2cdm_automate.xsl 
   ```

**4.** The txt file for your XML file should now be in the Saxon folder on your desktop. Open Excel and then open the txt file you just created (note "All files" must be selected in order to see your new txt file). Select "Next", "Next", "Finish" on the 3 window Text Import Wizard prompt. 

Voila!

You can manipulate these fields to fit your needs. For example, use find and replace to change "hook_id" into item call numbers (ex: folder_1 to F-20367/1).  


# Excel formulas/tips

### Deleting empty cells

Home tab-->Find & Select-->Go to Special...-->Blanks 

Home tab-->Delete-->Delete cells 

### Breaking apart strings of text

Delimit by characters (will delimit by every instance of this character within the string) 

   Data tab-->Text to Columns-->Delimit-->Choose your delimiters 
   
By Formula (can delimit by only first instance of character) 

```
=LEFT(A1,FIND("[delimiter]",A1)-1)  

=RIGHT(A1,LEN(B1)-FIND("[delimiter]",A1)) 
```
 
**Example:**

T-40328/1 Mix 1  in column A 

To break apart by first space so you can have "T-40328/1" in one column and "Mix 1" in another, use  

```=LEFT(A1,FIND(" ",A1)-1) and =RIGHT(A1,LEN(B1)-FIND(" ",A1))``` 


# Arrangement

Archival papers and records are usually accessioned in groups called collections. Collections often divide into logical units of some sort, but the depth of our arrangement work largely depends on use. As such, we begin with a "first pass," which involves no arrangement.  

- **First Pass** (description of) 

- **Series/File:** If we decide to arrange a collection into smaller units, we want to establish a framework that will enable the researcher to see the various parts of a collection without losing sight of the whole. The parts are usually established as series, which may be further divided into subseries. Keep in mind, there is no rule that says you must have series. There are times, particularly with small collections consisting chiefly (but not necessarily exclusively) of materials of one type or format, you can simply list the files. Increasingly we do this with larger collections too, when the groupings are more like large files than holistic, self-contained series. 

- **Series arrangement statements** 

 - **Alphabetical**

- **Chronological**

- **Original order has been maintained**


# Drop in Numbering for Digitization Requests

Use a combination collection number, box number, and folder numbering in this syntax: 

00000_0000_0000 

So folder 1 in Box 12 of collection 40001 would be:

40001_0012_0001 
