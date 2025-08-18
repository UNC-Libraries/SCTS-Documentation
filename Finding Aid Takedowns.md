Created August 2025 by Dawne Lucas

# Procedures for Removing a Finding Aid from Archy

***

**Scenario 1: Removal requires the creation of a take-down page in the Unavailable Collections section:**

1. **Curator** creates a Jira ticket assigned to **Archival Technical Services** requesting the removal.
    - a. Suggested wording for a take-down page in the <a href="https://library.unc.edu/wilson/unavailable-collections/">Unavailable Collections</a> section should be included in the ticket (the wording might be edited by **Communications**).

    - b. If applicable, **Technical Services Archivist for Collection Management** will create a deaccession record in ArchivesSpace.

2. **TS-Archival** creates a Jira ticket assigned to **Capdev** so there is a record of the work and notify **Emily Brassell** and/or **Steve Segedy**.

    - a. Attach the existing finding aid PDF (download from Archy) to the Jira ticket. Save the PDF to LOUIS.

3. **UX/Communications** creates a take-down page in the <a href="https://library.unc.edu/wilson/unavailable-collections/">Unavailable Collections</a> section.

4. **UX** adds a link to the take-down page on the <a href="https://library.unc.edu/wilson/unavailable-collections/">Unavailable Collections</a> page.

5. **TS-Archival** deletes the finding aid from Archy via Pipette.

6. **TS-Archival** un-publishes (_not_ delete) the resource record in ArchivesSpace.

    - a. Add an explanation to the Repository Processing Note field located near the top of the resource record.

7. **Capdev** adds <a href="https://unclibrary.atlassian.net/wiki/spaces/capdev/pages/45431578/Managing+URL+Redirects+on+Library+Servers">rewrite rule to apache config</a>, sending requests for the finding aid URL to the new take-down page.

8. **Capdev** tests rewrites and asks **IMS** to commit this change to SVN.

9. **Capddev** records deacession in <a href="https://unclibrary.atlassian.net/wiki/spaces/capdev/pages/45444787/Finding+Aids+-+Deaccession+Procedures">Jira documentation</a>.

10. **TS-Archival** creates a Jira ticket for **Bibliographic Technical Services** for MARC record removal.
    - a. Steps 11a and 11b (below) should be included in the ticket. Include both steps unless absolutely sure which one applies.

11. **TS-Biblio** will proceed as follows:

    - a. If the collection has a collection-level record coded “Notautho” and without an OCLC number then it has not been counted in cataloging statistics and can just be deleted from Sierra.
    - b. If the collection has a record that has been added to OCLC, remove our holdings from OCLC.  Using the “Report Error” function, send a message to OCLC notifying them that the record can be deleted because UNC no longer holds the collection.  Notify Joe Copp with the item record number that should be withdrawn.  He will code this as withdrawn and suppress the bibliographic record.

--

**Scenario 2: Removal does not require the creation of a take-down page in the Unavailable Collections section:**

1. **Curator** creates a Jira ticket assigned to **Archival Technical Services** requesting the removal.

    - a. If applicable, **Technical Services Archivist for Collection Management** will create a deaccession record in ArchivesSpace.

2. **TS-Archival** creates a Jira ticket assigned to **Capdev** so there is a record of the work and notify **Emily Brassell** and/or **Steve Segedy**.
    - a. Attach the existing finding aid PDF (download from Archy) to the Jira ticket. Save the PDF to LOUIS.

3. **Capddev** records deacession in <a href="https://unclibrary.atlassian.net/wiki/spaces/capdev/pages/45444787/Finding+Aids+-+Deaccession+Procedures">Jira documentation</a>.

4. **TS-Archival** deletes the finding aid from Archy via Pipette.

5. **TS-Archival** un-publishes (not delete) the resource record in ArchivesSpace.
    - a. Add an explanation to the Repository Processing Note field located near the top of the resource record.

6. **TS-Archival** creates a Jira ticket for **Bibliographic Technical Services** for MARC record removal.
    - a. Steps 7a and 7b (below) should be included in the ticket. Include both steps unless absolutely sure which one applies.

7. **TS-Biblio** will proceed as follows:
    - a. If the collection has a collection-level record coded “Notautho” and without an OCLC number then it has not been counted in cataloging statistics and can just be deleted from Sierra.
    - b. If the collection has a record that has been added to OCLC, remove our holdings from OCLC.  Using the “Report Error” function, send a message to OCLC notifying them that the record can be deleted because UNC no longer holds the collection.  Notify Joe Copp with the item record number that should be withdrawn.  He will code this as withdrawn and suppress the bibliographic record.
