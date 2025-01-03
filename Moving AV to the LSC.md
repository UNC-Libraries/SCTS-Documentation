# Overview

- [Introduction](#introduction)
- [Jitterbug Data](#jitterbug-data)
- [Barcoding](#barcoding)
- [Templating and Creating MARC Records](#templating-and-creating-marc-records)
- [Quality Control](#quality-control)
- [Shipping Films](#shipping-films)

***

# Introduction
Below is documentation of our current workflow for barcoding and relocating motion picture film materials to climate-controlled storage at the Library Services Center (or LSC). After rehousing the films that you are working with (information about this process can be found in our [audiovisual materials processing documentation](https://github.com/UNC-Libraries/SCTS-Documentation/blob/main/Audiovisual%20Materials.md#rehousing-materials)), the next major steps involve retrieving metadata for these materials from Jitterbug, attaching barcode labels to the items, adding barcode data to the metadata spreadsheets and communicating with various stakeholders to generate MARC records and arrange transportation before finally bringing the materials out to the LSC. It might seem like quite a bit, but it’s a pretty smooth process once you get into the swing of things! 

**Why Relocate to Cold Storage?**

In short, relocating films from the Wilson Library stacks to climate-controlled storage at the LSC is primarily a preservation-related concern. Like all collection items, motion picture films react to heat and humidity present in the storage environment. For the most part, the motion picture materials held at Wilson Library have either an acetate or a polyester base: each of which reacts differently to unstable environmental conditions. In the case of acetate-based films, heat and humidity can cause the film base to release acetic acid: a condition popularly referred to as vinegar syndrome. The buildup of this acetic acid over time results in shrinkage and embrittlement of the film base, which can ultimately result in the film becoming completely unusable. Furthermore, this process is autocatalytic, which means that the acetic acid gas released by these films can affect other materials stored nearby; for this reason, vinegar syndrome is a major threat to the long-term viability of our motion picture collection as a whole. Polyester films, on the other hand, are significantly more stable than acetate-based films but can still be affected by improper storage conditions: with the most common symptoms being film shrinkage and color fading. Unfortunately, a recent environmental survey indicated that the environmental conditions present in the stacks at Wilson Library are insufficient for the long-term retention of motion picture materials. For this reason, we have determined that the best way to ensure the overall longevity of our motion picture materials is by relocating them to climate-controlled storage at the LSC. 

# Jitterbug Data
As discussed in our [audiovisual materials processing documentation](https://github.com/UNC-Libraries/SCTS-Documentation/blob/main/Audiovisual%20Materials.md#jitterbug), we use an internal database system called [Jitterbug](https://jitterbug.lib.unc.edu/) to store and track metadata pertaining to Wilson’s archival audiovisual materials. The use of this program has numerous applications that aid in everything from archival processing to management of our ongoing AV digitization projects. In this case, we are using it to retrieve the metadata that will eventually be used to create the MARC records for each object. These MARC records will allow the items to be tracked via the library catalog which, in turn, means that they are eligible for storage at the LSC. 

Once you have logged into Jitterbug, you will see three buttons at the top of the page: “Audio Visual Items”, “Preservation Instances” and “Transfers”; each of which directs you to a series of records. For our purposes, the “Audio Visual Items” tab is the only one to be concerned with since we are focusing solely on data pertaining to the physical items themselves rather than digitized content (which is the primary focus of the “Preservation Instances” and “Transfers” tabs). Click on the “Audio Visual Items” button to retrieve the metadata for the your items.

The typical approach to pulling down item metadata involves approaching these materials on a collection-by-collection basis, using the content filters visible on the left side of the screen. Jitterbug offers four different filters for materials: “Preservation Instance” filters, “Type” filters, “Collection” filters and “Format” filters. For our purposes we only need to concern ourselves with the “Type” and “Collection” filters.
![Film metadata in Jitterbug](https://github.com/andrewdcrook/Photographs/blob/main/Picture1.jpg)  
Since we are only working with film items, check the “Film” box under “Type Filters”. From there, scroll through the collections featured under “Collection Filters” until you find the collection that you will be working with.  
Once the correct collection has been selected, hold down the shift key and click the first item that you intend to work with, then click the last item of this intended group: this should highlight all the records that you will be exporting. After this is done, click the “Batch” button (located at the top of the page) and select “Export” from the dropdown menu that appears.
![Selected film data in Jitterbug](https://github.com/andrewdcrook/Photographs/blob/main/Picture2.jpg)  
A box should appear containing a list of fields to export. For the moment, it’s all right to click “Select All”. After that, click “Build and Download” and a CSV document containing the compiled data should be downloaded to your machine. 
![Film export data fields in Jitterbug](https://github.com/andrewdcrook/Photographs/blob/main/Picture3.jpg)

# Barcoding
Once you have downloaded the CSV spreadsheet, the first thing to do is to save the file as an Excel workbook: I prefer to name these files with the collection number and “ToMARC” at the end, i.e. “20193_ToMARC”. Once this is done, insert a new column to the left of the call number column on the spreadsheet; this is where the barcode data will be added. Once this column has been created, make sure to format it as text; this will ensure that the leading zeroes in the barcode number are retained after scanning. 

At this point, with your films properly rehoused and your spreadsheet open on your desktop you should be ready to start barcoding! 

A quick note on the barcode stickers: Technical Services should have a healthy supply of barcode stickers available, but if that isn’t the case contact Resource Description and Management (RDM) staff (as of this writing, our contact is Kim Allen) and they should be able to provide additional materials. 

The process of barcoding films is relatively straightforward, but it does require a degree of diligence. At this point, we’re using a USB powered scanner attached to a laptop or desktop to add barcode data into the spreadsheet. Select the cell in the barcode column that is directly adjacent to the call number of the item that is being barcoded; if the cell has been formatted as ‘text’ then it should be able to record the entire barcode, including the leading zeroes that are otherwise removed.  To enter the data, press the tip of the scanner onto the barcode sticker and rub horizontally across the barcode until the device beeps; if all has worked correctly, the barcode data should appear in the selected cell. Once you have completed scanning the sticker make sure to check this cell to ensure that all numbers (including leading zeroes) have been logged and that the information present in the spreadsheet matches what is on the barcode sticker. This will ultimately help to prevent any problems down the line once the items have been delivered to the LSC. After entering the barcode information, peel the sticker from the sheet and attach it to the side of the film can, preferably to the left of the call number label on the container. Continue to repeat this process until all film cans have barcode stickers attached and the accompanying spreadsheet has barcode data in the appropriate spots. 
![Barcoded film cans in library stacks](https://github.com/andrewdcrook/Photographs/blob/main/Picture4.jpg) 

# Templating and Creating MARC Records
Once the barcode data has been logged, the next step is to work with Resource Description and Management (RDM) staff to create MARC records for each film; as of this writing, our primary contacts are Wanda Gunther (authority control and database management librarian) and Thuy-Anh Dang (metadata librarian for media resources). A key part of this process is to move the data from our initial metadata spreadsheet downloaded from Jitterbug into a templated spreadsheet that RDM will use to import this information into Sierra (our current cataloging system); a blank copy of this templated spreadsheet can be found on the G drive by following this folder path: G>wilson>ts>archival_cataloging>Films_ToMARC-Template.xslx. 
![MARC data template spreadsheet](https://github.com/andrewdcrook/Photographs/blob/main/Picture5.jpg)

For the most part, the fields in the MARC template spreadsheet should correspond one-to-one with the fields in the metadata spreadsheet; however, there are a few things that might seem initially confusing, so we’ll go through the fields here from left to right. 

**The first three fields are marked 949\\, 949 \1 $z and 915 \\:** these are strictly for MARC record formatting; the data in these fields should be pre-populated in the initial template document and can be cut and pasted as needed. 

**949 \1 – CallNumber:** Corresponds to “CallNumber” in our original spreadsheet

**949 \1 $i – Barcode:** Corresponds to “Barcode” in our original spreadsheet

Following these fields are three fields marked “245 02 $a”, “245 03 $a” and “245 04 $a”: these fields can be left blank

**245 00 $a – Title:** Corresponds to “Title” in our original spreadsheet

**300 \\ $a:** This field is for indicating the number of items in a film can. Data in this field should be formatted as follows: 1 film reel ; $c (for an item that has only one film in the can) and adjusted accordingly if more items are present in the can (2 film reels ; $c for an item with two reels in a container, for instance). 

**500 \\ $a – Collection Name:** Place the collection name as found at the top of the finding aid.

**500 \\ - Collection #:**  Place the collection number as found at the top of the finding aid; make sure to retain the leading zero for Southern Historical Collection items

**500 \\ - ItemYear:** Data from the ItemYear or ItemDate fields can be placed here. If entering a specific date in the field be sure to reformat the data from the YYYY-MM-DD format to a Day Month Year format, so 1956-11-02 becomes 2 November 1956, for instance. 

**500 \\ - ContainerNote:** Corresponds to ContainerNote

**500 \\ - Base:** Corresponds to Base

**500 \\ - ContentDescription:** Corresponds to ContentDescription

**500 \\ - Element:** Corresponds to Element

**500 \\ - Color:** Corresponds to Color

**500 \\ - SoundType:** Corresponds to SoundType

**500 \\ - LengthInFeet:** Corresponds to LengthInFeet

**830 \0 – OriginalCollection:** Describes the original collecting unit for each item. At this time, the field can be populated with five options: “SFC Film Collection,” “SHC Film Collection,” “UARMS Film Collection,” “NCC Film Collection” and “RBC Film Collection.”

Once this data has been crosswalked to your satisfaction, it can be forwarded to RDM staff who will create the MARC records. After RDM staff verifies that the MARC records have been added to the catalog, we can start performing quality control. 

# Quality Control
On the surface, this is a relatively straightforward step in the process: reviewing individual, newly created MARC records to make sure that the data that is in the templated spreadsheets is also present in the actual records. Typically, we try to QC a representative sample of the newly created records: for instance, with a batch of 500 records, we will want to check one out of every 10 or with a batch of 200 records we will inspect one out of every five. 
![Sample MARC record preview in Sierra](https://github.com/andrewdcrook/Photographs/blob/main/Picture6.jpg) 
The process of locating newly created records in Sierra is relatively straightforward. The first thing that you should see in Sierra after logging in is a search bar at the center of the screen with a dropdown menu directly to the left: click the dropdown menu in the top left corner and select Local/Dewey Call Number and enter the call number for the item; if the item has a record present in Sierra, that record should appear right away in a preview window. Looking around this window (pictured above) you will see basic title, description, and series information about the object: double check to make sure that this information lines up with what is present on the template spreadsheet that was forwarded to RDM. In addition, be sure to check the bottom of this page to make sure that the call number and barcode data also matches what was submitted. 
 
Clicking the ‘View’ button located in the upper right corner of the window opens the full MARC record; this allows you to view some of the more specific descriptive elements that were part of your original spreadsheet. Again, this is just a matter of comparing the information that is present on the MARC record with what is on the spreadsheet that was submitted to RDM. 
![Full MARC record on display in Sierra](https://github.com/andrewdcrook/Photographs/blob/main/Picture7.jpg)
After completing quality control of your selected records, you should reach back out to RDM staff and inform them of any problems present with the records; if any issues do arise, make sure to check the records again following completion of corrections to confirm that the requested changes have been made. Once the records are in suitable condition for long-term retention, inform RDM that the records can be moved along; after this, wait a few days before actual shipping to ensure that the records are fully integrated into the system. 

# Shipping Films
After the MARC records have been loaded into the system, we can start planning to move the items to the LSC. The first step is to alert Circulation staff that we are going to be delivering materials to the LSC: as of this writing, our primary contact is Matt Welborn (Transfer and LSC Manager); this is done so that LSC staff is aware of our delivery and to inform us of any issues that might prevent us from making a delivery at that time. Typically, we reach out about this roughly a week before we deliver the items to the LSC: this provides us with extra flexibility to arrange transportation and moving assistance. 

Once our move date is confirmed by Circulation, we can go ahead to arrange transportation. Typically, we reach out to the Davis Library mailroom clerk (Christine Zimmerman is in this position as of this writing) to see if we can borrow one of their full-sized vans (which can hold up to around 500 reels).  

In the time between arranging the shipment and the actual move, your primary concern should be to ensure that the materials are easy to move through the loading dock on Level 2 and that you have enough supplies and assistance to allow the move to proceed smoothly. For the most part, audiovisual materials, including films, are stored on Level 10 of Wilson Library. For this reason, we will want to stage all the films somewhere on Level 2 prior to shipment. For the most part this is relatively straightforward and can be done by a single person over the course of a few hours a day or two before moving the films to the LSC. There are several spaces on Level 2 that can be used as temporary staging areas for films: namely Room 205 and the storage room located adjacent to that room. Regardless, relocating the films to these spaces will ultimately make the process of loading the van significantly easier. 

Soliciting volunteers will help to expedite the shipping process. For moving a group of around 500 films, a crew of 4 to 5 volunteers is ideal to load the van in an efficient manner: with two volunteers loading up flatbeds with items from staged storage, two volunteers loading the van from the flatbeds (with one volunteer handing off films from the cart and the other stacking the cans inside the van) and one volunteer roaming between the two groups helping as necessary. Typically, volunteers can be solicited via the “FYI-SC” channel in the Special Collections group on Teams. As with every step, this solicitation should happen a few days before the move to provide a degree of flexibility for potential volunteers. Once the materials have been placed in the back of the van, make sure to cover them with the pair of moving blankets that are usually stored in the stacks area adjacent to Room 206. Doing so will help reduce the likelihood of materials shifting and getting damaged or misplaced during shipment  . 

The actual transportation of materials out to the LSC should only require two people: one to drive and one to assist in unloading the van. The LSC is at 5 Anson Street in Durham: a destination that can be easily reached by taking I-40 to the Durham freeway. When arriving at the facility, back up to the first loading dock garage door (the one on the right) and park the van. From there, step out of the van and ring the doorbell located next to the side door. An LSC employee should let you in and open the garage door for you. After this, you should be able to back the van up to the loading dock and begin stacking the films on the carts located nearby. Make sure to stack the films with barcodes facing out as this will expedite the check-in process. The best approach to unloading films is to have one person in the back of the van handing off film cans to another person who then loads up the carts, with both people alternating positions periodically to reduce muscle strain. Once a cart is full, push it through the swinging doors into the LSC employee working space. Repeat this process until all cans have been removed from the van. 
