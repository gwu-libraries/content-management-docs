# Finding Aids

### Introduction

This policy is a guide to the creation of finding aid records in Alma; including steps for bibliographic record and electronic portfolio record creation. The primary purpose is to document the procedure to update and transform the MARCXML record, as well as which specific MARC fields need to be added in addition to or in place of standard cataloging procedures.

### Convert file to MRC / MRK

Special Collections will send a ticket to RDG through Salesforce and will include the exported MARCXML file from ArchiveSpace.&#x20;

After downloading the MARCXML file from Salesforce, open MarcEdit.

* Select MARC tools <img src="../../../.gitbook/assets/image (21).png" alt="" data-size="line">
* Once in MARC tools, settings are:
  * Select operation: MARC21XML => MARC21
  * Open... \[this is the finding aid file, usually beginning with MS...]
  * Save As... \[this is where you will want to save the file]
  * Default character encoding: UTF8
* Once all options are set, select "Execute"

{% hint style="info" %}
You do not need to exit out of the window once the process is complete. You can use the same window to process the MRC file into an MRK file. &#x20;
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (22).png" alt=""><figcaption></figcaption></figure>



For the next steps, the file will have to be transformed into MRK (MarcEdit binary format). Open a MARC Tools window if you've closed the previous one. The settings for this are:

* Select Operation: MarcBreaker
* Open... \[this is where you saved the MRC file]
* Save As... \[this is where you will save the MRK file]
* Default character encoding: UTF8

Once configured, select "Execute"

Once the process is complete, select "Edit Records"

<figure><img src="../../../.gitbook/assets/image (19).png" alt=""><figcaption></figcaption></figure>



### Editing the file in MARC Edit

The file that comes out of Archivespace requires a few changes that can be easily performed in MarcEdit. This adds in the most common 33X fields for finding aids, finding aids as a genre/form term, and corrects multiple fields. The tasklist is available <\<URL>> for download. The tasklist does the following

* ADD 336 \\\\$atext$btxt$2rdacontent$0http://id.loc.gov/vocabulary/contentTypes/txt
* ADD 336 \\\\$astill image$bsti$2rdacontent$0http://id.loc.gov/vocabulary/contentTypes/sti
* ADD 337 \\\\$aunmediated$bn$2rdamedia$0http://id.loc.gov/vocabulary/mediaTypes/n
* ADD 338 \\\\$aother$bnz$2rdacarrier
* ADD 655 \7$aFinding aids.$2lcgft$0http://id.loc.gov/authorities/genreForms/gf2014026103
* ADD 655 \7$aFinding aids.$2fast$0http://id.worldcat.org/fast/01919927
* COPY 856 TO 555
* DELETE 040
* ADD 040 $aDGW$beng$erda$cDGW
  * If the 040 has $edacs, add it back in
* SUBFIELD\_EDIT 049 $a https://library.gwu.edu/ REPLACE WITH DGWW









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

Electronic material type: Document<br>

### Finishing

Check to make sure that electronic portfolio is attached to the record, and that the finding aid link works.&#x20;

Once completed, notify Spec staff that record is completed.&#x20;
