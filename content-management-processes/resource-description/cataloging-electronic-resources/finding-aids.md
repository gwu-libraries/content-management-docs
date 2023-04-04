# Finding Aids

### Introduction

This policy is a guide to the creation of finding aid records in Alma; including steps for bibliographic record and electronic portfolio record creation. The primary purpose is to document the procedure to update and transform the MARCXML record, as well as which specific MARC fields need to be added in addition to or in place of standard cataloging procedures.

### Summary of Steps

* Spec staff provide MARC21XMLl file download and convert to marc21 file using MARCEdit
* Convert mrc to mrk file using MARCedit (capture the title)
* Import mrc file to OCLC Connexion online save file (do not delete original file)
* Update record as necessary
* Notify Spec staff about typos and subject headings changed or added; data will need to be corrected in ASpace;&#x20;
* Export from OCLC Connexion to local dat file
* Convert dat to mrk using MARCedit
* Convert mrk to mrc using MARCedit
* Use import profile to add record to NZ and IZ
* Add electronic portfolio holding to IZ record
* Notify Spec staff that record is in Alma with portfolio holding
* Spec staff are responsible for adding holding record to track movement of physical materials

### Editing record imported into OCLC

#### Fixed field information

* Desc should be i
* Ctry should be dcu
* Dates (should match data in both fields 245, 520)

#### Body of record (MARC fields)

* 040 String must include: DGW ǂb eng ǂe rda ǂc DGW. May include ǂe dacs (Spec staff supply)
* 099 9/ Local call number&#x20;
* 041 eng Remove from OCLC version of record if eng is the only language of the materials involved&#x20;
* 245, 300, 520, 524, 541, 6xx (edit as appropriate)
* 33x, 555, 6xx Add as needed

### Import Bibliographic record into Alma both NZ and IZ

Use import profile Gelman Stacks Load Bib Records (books)

### Alma Electronic Portfolio

{% hint style="info" %}
For information about adding an electronic portfolio, please go to << ADD LINK >>
{% endhint %}

Part of an Electronic Collection: George Washington University Special Collections Research Center Finding Aids

URL: https://searcharchives.library.gwu.edu/repositories/2/resources/\[finding aid ID number]

Electronic material type: Document\


### Finishing

Check to make sure that electronic portfolio is attached to the record, and that the finding aid link works.&#x20;

Once completed, notify Spec staff that record is completed.&#x20;
