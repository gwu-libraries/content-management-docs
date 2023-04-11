---
description: '*copy editing and formatting still needs to be finished'
---

# Cataloging Physical Items

## Introduction

This documents the process for basic copy cataloging for all cataloging and specifically for physical monographs entering in the general circulating collection. While this is the basis for all cataloging, there are more involved procedures for electronic resources, Special Collections and GRC, etc. Where document conflicts, follow the more specific documentation.&#x20;

## Copy cataloging (Alma)

Search Alma IZ All Titles to find a record. A record should exist for pretty much everything that goes through the regular cataloging process, but in many cases it will be a brief/stub record

* Search by ISBN if the item has one; otherwise use keyword title; otherwise use item barcode
* When you find a record, take a look at it to see what it looks like (is it complete, is it a brief record with information for the cataloger like collection names, etc?), and see if the record is linked to the NZ

Search Alma NZ All Titles to see if a record exists in the NZ for the resource

* Using ISBN, keyword, OCLC number or other information from the IZ record
* If a match exists, make sure it’s for the same manifestation (same format, edition, date, etc.)

If there is a properly matching record that is not already linked to the IZ record, open the IZ record in Metadata Editor

* If there is institution-specific or copy-specific metadata in the IZ record (such as a collection name or donor note), move that information to the proper local extensions (Alma local fields) before linking to the NZ
* Choose Record Actions>Share with network. When alerted that matches are found, view matches and select “Link” for the correct NZ record

Search OCLC Connexion for the resource

* Identify the correct record - format, language, isbn, correct title, rda record, call number, subject headings, existence of DLC, number of holdings, whether GW has holdings
* If GW has holdings on the wrong record, remove holdings and add them to the correct record
* If GW does not have holdings, add holdings to correct record
* Compare OCLC record with NZ record to determine if NZ record should be updated
* Do copy cataloging process (or original cataloging process) in Connexion

<< add details about which fields we check for what and what we do at minimum >>



If the OCLC record is changed from the Alma NZ-linked record, or if only Alma IZ record exists:

1. MD Editor>Search Resources
2. Look up record by OCLC number
3. Copy & Merge
4. Save record
5. Add 973 and any bib local notes (961, 962, 963, 971, 975, etc)
   1. You can use your template (update as needed) and Editing Actions>Expand from Template (Ctrl+E), or manually enter the non-973 fields if preferred
6. If record is not yet linked to NZ, share with network
7. View related data>Inventory
   1. Compare the bib call number with holding call number
   2. If edits to call number are needed, or if notes need to be added to holding record, edit holding record
   3. Manually add notes needed, or use a template
8. Check shelflist from bib record, adding cutter
   1. If needed, add 090 with local call number & update holding record call number from bib (Alt+U)
   2. Pencil in call number, including prefixes based on location
9. Save & release holding
10. Edit item record
    1. Add receive date if none exists
    2. Make sure material type is accurate
    3. Make sure Chron, Enum, Description are accurate
    4. Make sure no temp location
11. Save & release bib record (Ctrl+Alt+R)
12. Scan in items
    1. Done item or set status to physical processing
13. Deliver the item to its destination or to its destination shelf in 103
