Updated June 2020.

# Overview

- [Acquisition Information](#acquisition-information)
- [Dates](#dates)
- [Extent](#extent)
- [Items Separated](#items-separated)
- [Processing and Revision Notes](#processing-and-revision-notes)
- [Restrictions](#restrictions)
- [Abstract](#abstract)
- [Subject Headings](#subject-headings)
- [Capitalization and Punctuation](#capitalization-and-punctuation)
- [People and Place Names](#people-and-place-names)
- [Spell check](#spell-check)
- [Transformation and Review](#transformation-and-review)

***

# Acquisition Information

- Include all accession numbers for processed materials at the collection level. 

  - UA: **Transferred from department name in month year (RT number).**

  - Other: **Received from donor name in month year (Acc. number).**

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

# Items Separated

- Include all materials housed separately in the stacks and stored digitally. 

- For additions: Check existing numbering to make sure you start with the correct number. 

  - **Audiocassettes (C-05700/1-84)**
  - **Image Folders (PF-05723/1-/376)**
  - **Photograph Albums (PA-00613/1-19)**
  - **Oversize paper folders (XOPF-3824/1, OPF-3824/2-3)**
  - **Digital folders (DF-40283/1-20)**

# Processing and Revision Notes

- Update when making revisions to existing finding aids. In the revision note, also record the last folder/format numbers used: 

```
<revisiondesc>
<change>
<date></date>
<item>Updated for addition of DATE (Acc. XXXXXX) by NAME</item>
</change>
<revisiondesc> 
```

- See boiler plate processing statements in [Descriptive Elements](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/master/Descriptive%20Elements.md#processing-information).

```<processinfo></processinfo> (viewable to public)```

# Restrictions

- Check control files and ArchivesSpace. 

- Note at every level—collection, series, and container. 

- Remove outdated restrictions and “This collection contains unprocessed…” (if applicable). 

- Word consistently and explicitly. Use boiler plate restriction statements found in [Descriptive Elements](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/master/Descriptive%20Elements.md#restrictions)

- Restrictions to Access statement for A/V: **Use of audio or moving image materials may require production of listening or viewing copies.**


# Abstract

- Include contextual information in the first sentence of the 520 abstract, as appropriate. 

- Include ethnic and racial identities for creator(s), collector(s), and major figures documented in collections so that whiteness is no longer the presumed default of the people represented in our collections. Consult the [Style Guide](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/master/Style%20Guide.md) for a list of recommended ethnic and racial identities. 

- For additions: add information to abstract, as needed. 

- Conscious editing: When appropriate, re-frame the abstract narrative to surface and emphasize the lives of those historically left out of our description. Consult [Principles for Ethical Description](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/master/Principles%20for%20Ethical%20Description%20in%20Special%20Collections%20Technical%20Services.md), [Style Guide](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/master/Style%20Guide.md#abstracts-collection-overview-bioghist-notes), and [Descriptive Elements](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/master/Descriptive%20Elements.md#scope-and-content-note-and-abstract) for further information. 

# Subject Headings

- Be sure to include a heading for the creator

- End with a period, with at least two exceptions: 

  - Open-ended dates, e.g., **Davis, Angela Y. (Angela Yvonne), 1944-** 

  - Information in parentheses, e.g., **Guitar music (Blues)**

# Capitalization and Punctuation

## Series titles

- End with a period.

- Use title capitalization: **Series 2. Financial and Legal Papers, 1685-1887.** 

- Style for series titles in additions:  **Series 3A. Annual Reports, 1921-1922 (Addition of 2016).** 

- If the collection consists of only one series collections, the series title is the same as collection title and the series is not numbered. 

## Unittitles

- No ending punctuation.

- Use commas, not colons, before dates.

- Use sentence capitalization: **Miscellaneous short writings, 1856-1857 and undated


# People and Place Names

## People

- Choose one form of a name and use it consistently throughout the finding aid. 

## Places

- Where proceeded by city or county, use appropriate abbreviations: **She was born in Birmingham, Ala.** 

- Put commas around the abbreviated state name: **She stopped by Oxford, Miss., on her way to Los Angeles, Calif.**  

# Spell check

Run it over your whole XML document.

# Transformation Review

Take one last look at the HTML document to make sure you do not have any special characters interrupting the display. See Special Characters in [EAD](https://github.com/UNC-Libraries/TS-Archival-Procedures-Manual/blob/master/EAD.md#special-characters) for help.

**This Finding Aid Checklist was modified from [Checklist Mock-up](https://adminliveunc-my.sharepoint.com/personal/ljcb_ad_unc_edu/Documents/Checklist%20Mockup.docx) in June 2020.**
