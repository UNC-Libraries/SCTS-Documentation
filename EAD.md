# Overview

- [Container Types](#container-types)
- [Find and Replace with Regular Expression](#find-and-replace-with-regular-expression)
- [Container Numbers hook-I.D.](#container-numbers-hook-id)
- [Extent (overriding "approximately")](#extent-overriding-approximately)
- [Unsuppress a Container Number](#unsurpress-a-container-number)
- [Special Characters](#special-characters)

***


# Container Types

Here is the list of container types for the _type_ attribute in the `<container>` tag (note that this attribute is case sensitive). Anyone needing another type of container can ask Lynn to expand the list.   

| **Display Names**                              | `<container type=>`     | Invidual Item/Folder/Box Style        |
| ---------------------------------------------- | ------------------------| ------------------------------------- | 
| **8-Track Tape**                               | 8t                      | 8T-#                                  |
| **Audiocassette**                              | audiocassette           | C-collection#/item#                   |
| **Audiodisc**                                  | audiodisc               | D-collection#/item#                   |
| **Audiotape**                                  | audiotape               | T-collection#/item#                   |
| **Audio Box**                                  | audiobox                | AB-collection#/item#                  |
| **Box**                                        | box                     | box#                                  |
| **Card File**                                  | cardfile                | CF-collection#/item#                  |
| **CD Listening Copy**                          | cdlc                    | Unique ID keyed to original format    |
| **Data Compact Disc**                          | datacd                  | DCD-collection#/item#                 |
| **Data Digital Video Disc**                    | datadvd                 | DDVD-collection#/item#                |
| **Digital Audio Tape**                         | dat                     | DAT-collection#/item#                 |
| **Digital Item**                               | digitem                 | DI-collection#/item#                  |
| **Digital Folder**                             | digifolder              | DF-collection#/item#                  |
| **Digital Video Disc**                         | dvd                     | DVD-collection#/item#                 |
| **Envelope**                                   | envelope                | envelope#                             |
| **Extra Oversize Image**                       | xoimage                 | XOP-P-collection#/item#               |
| **Extra Oversize Image Folder**                | xoimagefolder           | XOP-PF-collection#/folder#            |
| **Extra Oversize Paper**                       | xopaper                 | XOP-collection#/image#                |
| **Extra Oversize Paper Folder**                | xopaperfolder           | XOPF-collection#/folder#              |
| **Film**                                       | film                    | F-collection#/image#                  |
| **Flat Box (NCC Photo Archives only**          | flatbox                 | box#                                  |
| **Flat File Drawer (NCC Photo Archives only)** | flatfile                | drawer#                               |
| **Flat Storage Image (8x10)**                  | o0810image              | PColl#/uniqueID                       |
| **Floppy Disc**                                | fkd                     | FLD-collection#/item#                 |
| **Folder**                                     | folder                  | folder#                               |
| **Framed Item**                                | fr                      | FR-collection#/item#  PColl#/uniqueID |
| **Image**                                      | image                   | P-collection#/item#                   |
| **Image Box**                                  | imagebox                | IB-collection#/box#                   |
| **Image Folder**                               | imagefolder             | PF-collection#/folder#                |
| **Instantaneous Disc**                         | fd                      | FD-collection#/item#                  |
| **Interview**                                  | interview               | interview#                            |
| **Item**                                       | item                    | item#                                 |
| **Lantern Slide**                              | lantern                 | LS-collection#/item#  PColl#/uniqueID |
| **Mini-Disc**                                  | md                      | MD-collection#/item#                  |
| **Museum Item**                                | museumitem              | MU-collection#/item#                  |
| **Music Compact Disc**                         | cd                      | CD-collection#/item#                  |
| **NCC Reference Box**                          | pref                    | Box#                                  |
| **Optical Disc Cartridge**                     | odc                     | ODC-collection#/item#                 |
| **Oversize Box**                               | obox                    | OB-collection#/item#                  |
| **Oversize Image**                             | oimage                  | OP-P-collection#/item#                |
| **Oversize Image Folder**                      | oimagefolder            | OP-PF-collection#/image#              |
| **Oversize Paper**                             | opaper                  | OP-collection#/item#                  |
| **Oversize Paper Folder**                      | opaperfolder            | OP-PF-collection#/image#              |
| **Oversize Volume**                            | ovolume                 | SV-collection#/item#                  |
| **Photograph Album**                           | photoalbum              | PA-collection#/item#  PColl#/uniqueID |
| **Reel**                                       | reel                    | reel#                                 |
| **Roll Film Box (NCC Photo Archives only)**    | rollfilmbox             | box#                                  |
| **Rolled Item**                                | roll                    | R-collection#/item#                   |
| **Separated Folder (i.e. vault item)**         | separatedfolder         | SEP-collection#/folder#               |
| **Song Folio**                                 | folio                   | song folio#                           |
| **Special Format Image**                       | sfimage                 | SF-P-collection#/item#                |
| **SFC Audio Cassette**                         | sfaudiocassette         | FS-collection#/item#                  |
| **SFC Audio Open Reel**                        | sfaudioopenreel         | FT-collection#/item#                  |
| **Track**                                      | track                   | TR-collection#/track#                 |
| **Transcription Disc**                         | trans                   | transcription disc#                   |
| **Transcription Volume**                       | transv                  | TV-collection#/item#                  |
| **Unit**                                       | unit                    | unit#                                 |
| **Use Copy**                                   | uc                      | UCyear_item#                          |
| **Videodisc**                                  | videodisc               | VD-collection#/item#                  |
| **Videotape**                                  | videotape               | VT-collection#/item#                  |
| **Wire Recording**                             | wr                      | WR-collection#/item#                  |


# Find and Replace with Regular Expression

Using Regular Expression in Oxygen to create a **POWERFUL & SMART** “find and replace” search string:  

From time to time while processing, we have all come across changes that need to be made to the EAD that only effect the tags we are using, not the metadata between the tags.  

Example:

**Take→**

![Initial record with tags that require changes to the code](https://user-images.githubusercontent.com/58087302/78701037-50aaeb80-78d4-11ea-9431-9e1275d6c43a.jpeg "Example needing change")

**Change it to→**

![Changed record with improved tags](https://user-images.githubusercontent.com/58087302/78701232-abdcde00-78d4-11ea-8f50-06546165d184.jpeg "Example with changes")

In this example, I want to **remove the `<emph render=”doublequote”>` from the scope content notes (Location and Photographer) but NOT from the `<unittitle>`**. In this particular finding aid, there are tens of thousands of entries; each with different locations and photographers. Add to it that I **don’t want to touch the other `<emph render=”doublequote”>` tags in each entry.** The solution is using the REGULAR EXPRESSION feature available in the Oxygen “Find and Replace” feature. First, let me state: I AM NOT A PROGRAMMER in any sense of the word, but I have spent the last few years learning about Python and Regular Expression and how they can be used to navigate the world of EAD/XML especially in regards to the creation of POWERFULL search features.  

I will show how to use Regular Expression within Oxygen to make the changes shown above.  

1. Open the .xml you are going to be making the changes to in Oxygen.  

2. Find an example of the metadata that needs to be changed within the .xml file 

**See Example→**

![Highlighted text](https://user-images.githubusercontent.com/58087302/78701716-7dabce00-78d5-11ea-8ad1-3c0f981f43b2.jpeg "Example within instructions 1")

3. Select “Find” from options at top of window and select “Find and Replace” 

4. Under “Options” check “Regular expression” and “dot matches all”  

**See Example→**

![Windowed text 1](https://user-images.githubusercontent.com/58087302/78702032-f3179e80-78d5-11ea-841a-d831f578122f.jpeg "Example within instructions 2")

In this case, what I want to do is strip out the `<emph render=”doublequote”>` and `</emph>` tags from the scope content portion and nowhere else. In this case, all of the tags I am looking to replace are nested in "p" tags found within the scopecontent feature. This is a great use for regular expression.  

Simply put, Regular Expression is a set of special (predefined) characters that can be used to parse stings of characters and identify patterns. It is more complex than that, but for our purposes, this is good. (There are lots of sites out there but check out : http://www.regular-expressions.info/reference.html)  

5. Here is how the find and replace should be formed: 

**See Example→**

![Windowed text 2](https://user-images.githubusercontent.com/58087302/78702221-40940b80-78d6-11ea-8d35-b7ff6f07918e.jpeg "Example within instructions 3")

In the example above: In “Text to find” there are two uses of regular expression:  

- “ **.*?** ” → In this example, this is RE (Quantifier) for “everything in-between” the tags  
- “ **( )** “ → In this example, this is RE (Range) for “keep this string together”  

In the “Replace with” there is one use of regular expression:  

- “ **$1** ” → In this example, this is RE (String Replacement) that inserts whatever was “kept together” in the “Text to find” (above in find and replace)  

Created by Patrick Cullom.


# Container Numbers hook-I.D.

Correct item numbering makes finding aids JavaScript-hook compatible for future mass digitization using CONTENTdm interface. 

Letters can appear in single folder numbers but they cannot appear in ranges. For example, Folder 1a-2, is not allowed. 

For containers with prefixes, write as P-0345/1, P-0345/2 , and P-0345/3, rather than as a range: P-0345/1-3 even if they have the same unit titles. (via Laura Hart, January 2017) 

Do not encode multiple, non-sequential container numbers in the same `<container>`. For example, if both folder 14 and folder 18 have information on Martians, do not write `<container type='folder'>14, 18</container>`. In this case, you should encode them separately.(check with Lynn) 

Do not encode multiple unittitles in one c0x. We prefer multiple c0x with a repeating container, which is automatically suppressed so that you end up just seeing the multiple unittitles. 


# Extent (overriding "approximately")

Usually extent coding looks like this: 

```
<physdesc label="Extent">

<extent unit="items" encodinganalog="300">7000</extent> 

<extent unit="linear feet" encodinganalog="300">5.0</extent> </physdesc> 
```
 

If you have an exact item count and want to override "approximately" in the extent statement: 

Remove unit="items" from the first extent statement AND the entire second extent statement. Add the linear feet as a parenthetical after the item count. 

 

Code like this: 

```
<physdesc label="Extent"> 

<extent encodinganalog="300">6990 items (5.0 linear feet)</extent> </physdesc> 
```

# Unsupress a Container Number

Add altrender="display" to the container coding.

```
<c02><did><container type="box" altrender="display">11</container><unittitle>Volume 1-4</unittitle></did></c02> 
```

# Special Characters

Code ampersands &amp; OR &#38;. You can use "insert character" from the drop down menu in Oxygen.

Do not use curly quotes and/or apostrophes.  

Transform your document and check for funky characters in the html.
