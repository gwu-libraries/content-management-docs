# Cataloging Physical Items

Copy cataloging (Alma)

Search for title using title page of resource (not cover); prefer search using title over oclc # or isbn

Search both in NZ then in IZ  &#x20;

&#x20;   If title is in NZ and an unlinked bib in the IZ

Check our copy to see that publisher and date information match NZ record

&#x20;   If they match open IZ record in MDE (metadata editor)&#x20;

&#x20;   Under Record Actions tab choose→ Share with network this will generate a “matched records exist in the catalog do you want to view before saving” response. Choose “Yes” → when matching NZ record appears if it matches your piece&#x20;

Click “Link” then click Save button

Search for title again. The IZ record should now mirror the NZ record and the holdings in NZ should include GW’s copy.&#x20;

You can either add 973 fields manually in the MDE or choose to export the oclc record to a local dat file and use ME (marcedit) tool to add 973’s via a task created in ME&#x20;

If using ME after the 973 fields are added:&#x20;

Copy MMSID from IZ record and replace the oclc # in 001 field with it

&#x20;           Delete 003 field

&#x20;           Save file

Under ME Alma tab choose ”Update/Create”

Next Copy the oclc #.&#x20;

&#x20;       Search OCLC using the oclc # copied. Add our holdings to the record (hit F8 key)

Also search by title delete any holdings added to other records for the same title as                                       needed (Shift + F8 key)  &#x20;

&#x20; &#x20;

&#x20;       If title is not in NZ&#x20;

&#x20;           Choose “Manage sets” tab

&#x20;           Click “Add Set” choose itemized type and name your set

&#x20;           Choose Add members→ Add title  &#x20;

\


Next search for title in OCLC choose best record (match title, author, ISBN #,  place of publication, publisher, copyright date or date published). Note if date published is later than copyright date prefer record with later date.&#x20;

&#x20;           Update holdings (F8)

&#x20;           Export to local dat file

&#x20;           Open dat file with ME (metadata editor)

&#x20;           Run LD (linked data) task to record(s)

&#x20;           Run add 973 task to record(s)

&#x20;           Validate file

&#x20;           Copy MMSID from IZ record and replace the oclc # in 001 field with it

&#x20;           Delete 003 field

&#x20;           Save file&#x20;

&#x20;           Make sure the oclc # of the record you brought in from OCLC matches that on the record in our IZ. Update our IZ record oclc # if needed before continuing

&#x20;           Release the record in Alma&#x20;

&#x20;           Under ME Alma tab choose ”Update/Create” &#x20;

In Alma choose Run a Job tab→ search for “Link”&#x20;

&#x20;           Select your set&#x20;

&#x20;           In Enter task parameters screen check box→ Contribute IZ records

&#x20;           Submit

&#x20;           Confirm by title or oclc # search that record is&#x20;

In NZ and&#x20;

Includes 973 fields in IZ

\


Once bibliographic records and holdings for GW copy are in both NZ and IZ:

\


Check Holdings record for correct marc fields (852 and 866 as needed) with indicators, library  choice, location choice, complete call # with properly placed delimiters: Ex: 852 0/ \$$b gelman \$$c stacks \$$h HC79.C3 \$$i P76 2021 or \$$h HC79 \$$i .C3 2021

\


Check Item record for correct barcode, material type, item policy and permanent stacks location

\


If physical piece needs processing:

In Alma under Acquisitions Menu choose→ Scan in Items

In Set Status To box choose “Physical Processing”

Done button default should be “No”

In Scan item barcode box-->enter the barcode on the piece (manually or via scanner)

Place physical piece on “Physical processing” shelf in rm 103

\


If physical piece is shelf ready (ie has spine label, barcode) &#x20;

In Alma under Acquisitions Menu choose→ Scan in Items

In Set Status To box choose Anything it doesn’t matter what

Done button choose-->Yes

In Scan item barcode box-->enter the barcode on the piece (manually or via scanner)

Place physical piece on “Ready for shelving” shelf in rm 103
