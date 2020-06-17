# Overview

- [Acquisition Information](#acquisition-information)
- [Dates](#dates)
- [Extent](#extent)
- [Subject Headings](#subject-headings)
- [Items Separated](#items-separated)
- [Processing and Revision Notes](#processing-and-revision-notes)
- [Restrictions](#restrictions)
- [Special Characters](#special-characters)
- [Abstract](#abstract)
- [Capitalization and Punctuation](#capitalization-and-punctuation)
- [People and Place Names](#people-and-place-names)
- [Spell check](#spell-check)
- [Transformation and Review](#transformation-and-review)

***

# Acquisition Information

- Include all accession numbers for processed materials at the collection level. 

-- UA: **Transferred from department name in month year (RT number).**

-- Other: **Received from donor name in month year (Acc. number).**

- For additions: Also include RT and Acc. Numbers in Acquisitions Info tags at the series, file, or container levels, using the label “Acquisitions Information.” 

`<acqinfo><p>Acquisitions Information: Accession 20200617.1</p></acqinfo>`

# Dates

- Date ranges cover entire collection, series, etc.  

- Make collection dates consistent in the following tags: 

```
<titlestmt> <titleproper encodinganalog="title"> 

<frontmatter> <titlepage> <titleproper> 

<unittitle label="Title" encodinganalog="245"> 
```

- Formatted day month year: **3 June 1969**

# Extent

- Round numbers or remove the word “approximately”: **approximately 50** OR **52 items**

- Check the math across series to ensure that extents add up. Rounding up or down is okay. 

- For additions: add addition extent to collection level extent. 

# Subject Headings

- Be sure to include a heading for the creator

- End with a period, with at least two exceptions: 

-- Open-ended dates, e.g., **Davis, Angela Y. (Angela Yvonne), 1944-** 

-- Information in parentheses, e.g., **Guitar music (Blues)**

# Items Separated

Include all materials housed separately in the stacks and stored digitally. 

For additions: Check existing numbering. 

# Processing and Revision Notes

Update when making revisions to existing finding aids. In the revision note, also record the last folder/format numbers used: 

```
<processinfo></processinfo> (viewable to public) 

<revisiondesc>
<change>
<date></date>
<item>Updated for addition of DATE (Acc. XXXXXX) by NAME. Last folder (1001); imagefolder (PF-XXXXX/22; oversize folder (OPF-XXXXX/38</item>
</change>
<revisiondesc> 
```

# Restrictions

- Check control files and ArchivesSpace. 

- Note at every level—collection, series, and container. 

- Remove outdated restrictions and “This collection contains unprocessed…” (if applicable). 

- Word consistently and explicitly. Use Restriction templates found in [Descriptive Elements](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/master/Descriptive%20Elements.md)

- Restrictions to Access statement for A/V: **Use of audio or moving image materials may require production of listening or viewing copies.**


# Abstract

Include contextual information in the first sentence of the 520 abstract, as appropriate. 

Include ethnic and racial identities for creator(s), collector(s), and major figures documented in collections so that whiteness is no longer the presumed default of the people represented in our collections. Consult [Style Guide](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/master/Style%20Guide.md) for a list of recommended ethnic and racial identities. 

For additions: add information to abstract, as needed. 

Conscious editing: When appropriate, re-frame the abstract narrative to surface and emphasize the lives of those historically left out of our description. Consult [Principles for Ethical Description](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/master/Principles%20for%20Ethical%20Description%20in%20Special%20Collections%20Technical%20Services.md), [Style Guide](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/master/Style%20Guide.md), and [Descriptive Elements](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/master/Descriptive%20Elements.md) for further information. 


# Capitalization and Punctuation

## Series titles

End with a period.

Use title capitalization:

**2.1. Financial and Legal Papers, 1685-1887.** 

Style for series titles in additions:  

**2. Annual Reports, 1921-1922 (Addition of 2016).** 

For one series collections: the series title is the same as collection title. 

## Folder Titles

No ending punctuation.

Use commas, not colons, before dates.

Use sentence capitalization:

**Miscellaneous short writings, 1856-1857 and undated


# People and Place Names

## People
Choose one form of a name and use it consistently throughout the finding aid. 

## Places

Where proceeded by city or county, use appropriate abbreviations: **She was born in Birmingham, Ala.** 

Put commas around the abbreviated state name: **She stopped by Oxford, Miss., on her way to Los Angeles, Calif.**  

[From](https://adminliveunc-my.sharepoint.com/personal/ljcb_ad_unc_edu/Documents/Checklist%20Mockup.docx)

# Spell check

Run it over your XML document.

# Transformation Review

Take one last look at the HTML document to make sure you do not have any special characters interrupting the display. See Special Characters in [EAD](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/master/EAD.md) for help.
