# Overview

- [XML to TXT script](#xml-to-txt-script)
- [Excel formulas/tips](#excel-formulastips)
- [Drop in numbering for digitization requests](#drop-in-numbering-for-digitization-requests)


***


# XML to TXT script

Use the Saxon script to convert finding aid XML files to TXT files. This is an easy way to get finding aid data into a spreadsheet friendly format. Please note this script only exports limited fields from the XML file. At this time, nothing below the item title (i.e. `<genreform>`, `<scopecontent>`) can be exported through this script). The Saxon script exports the following fields from the XML file: 

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




# Drop in Numbering for Digitization Requests

Use a combination collection number, box number, and folder numbering in this syntax: 

00000_0000_0000 

So folder 1 in Box 12 of collection 40001 would be:

40001_0012_0001 
