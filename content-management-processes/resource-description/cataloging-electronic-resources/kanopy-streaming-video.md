---
description: Background and process for adding and deactivating licensed Kanopy videos.
---

# Kanopy Streaming Video

## Renewals

If a title is a renewal, it'll already be in Alma. In this case, you'll only have to update the coverage in the portfolio.

## New licenses

Titles that aren't currently in Alma are considered new licenses. That means that they will need to be brought in from OCLC and enhanced in MarcEdit to include portfolio URL, cover art URL, collection ID (for discovery collection), and cataloger notes.&#x20;

### Searching OCLC

* Using publisher number
  * This can be found on the SalesForce ticket, the command line search in OCLC is mn:\[insert number]. This is generally the quickest way to find a useable record for the title
* Using title, year, etc
  * If the publisher number didn't pull up a correct record for the Kanopy title, look for another record using other access points. Do not use the year of release, this is often different than what the Kanopy record has and can cause some incorrect matches. Note that the title that Kanopy provides is also not 100% accurate. It's always worth it to double check the actual streaming video for complete accuracy.&#x20;

### MarcEdit enhancements

If you want to import it into your MarcEdit, there is a [MarcEdit task list](https://drive.google.com/drive/folders/1Ub0bjJWjun8vrooX83A4GXt8GBejwaOM?usp=sharing) that will add URLs (you will have to update), the 787 for the Streaming Media collection, and the 973 cataloger information. The Sharepoint folder path is [GWLAI RDG](https://gwu0.sharepoint.com/sites/20180727030128000/SitePages/Home.aspx) > [MarcEdit](https://gwu0.sharepoint.com/sites/20180727030128000/Collaboration%20Items/MarcEdit) > [Tasklists](https://gwu0.sharepoint.com/sites/20180727030128000/Collaboration%20Items/MarcEdit/Task%20Lists).&#x20;

What the task list does:

1. Adds linked data
2. Deletes the following fields:&#x20;
   1. 856 (all conditions)
   2. 994 (all conditions
   3. 500 $a In process record
   4. 028s that don't contain $b Kanopy.&#x20;
3. Adds the following fields:&#x20;
   1.  787 \\\\$w81630409630004107$9LOCAL

       \*\* You can add in as many Discovery Collection IDs as desired, Alma will automatically add the title to each collection when importing.&#x20;
   2. 973 \\$aNew title ;$bCC ;$c\[cataloger name] ;$d\[YYYY-MM-DD]$9LOCAL
   3. 957 42$zCover Image$uhttps://www.kanopy.com/node/\[ID]/external-image$9LOCAL
   4. 40$u \[URL] $zA Kanopy streaming video
4. Build other system number field for Kanopy
   1. \=035 \\$a(CaSfKAN){028$a}, always add new field

Notes about the \[ ] fields

* \[URL] is where you will paste in the URL copied from the Invoice sent to SalesForce
* \[ID] is where you will paste the ID number taken from the URL
* \[cataloger name] is your last name
* \[YYYY-MM-DD] is the year, month, and day you're cataloging

When the record has all information updated and added, save as an MRC file.&#x20;

### In Alma

To import into Alma, use the "Kanopy" import profile. Once imported, update the license date in the portfolio in the "Coverage" fields.&#x20;



## Update tracking information

When Kanopy titles are imported or update, add in the information to the [tracking spreadsheet](https://gwu0.sharepoint.com/:x:/r/sites/20180727030128000/\_layouts/15/Doc.aspx?sourcedoc=%7BADE799FA-6AF1-4B9A-A212-B8853CC91183%7D\&file=Alma%20Ongoing%20Record%20Loads.xlsx\&action=default\&mobileredirect=true).&#x20;

