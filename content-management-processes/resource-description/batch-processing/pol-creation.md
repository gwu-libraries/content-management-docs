# POL Creation

{% hint style="info" %}
GWLAI staff use the GWLAI brief record/POL creation request [Google form](https://docs.google.com/forms/d/1ntU3X28emR-sJ0bSyIv8JW1mG5MrlsPtJdaxF9rT0DA/edit) when they are ready to place orders. RDG staff should set the notification on so they get alerts when a new request is submitted.
{% endhint %}

## Preparing the file

Put the new POL requests and column headings from the Google form into an Excel spreadsheet. If you export the Google sheet into an Excel format directly, be sure to delete all older requests.&#x20;



<figure><img src="https://lh4.googleusercontent.com/u7KxM2UrE98AInMWGlZsWV2LQTYrTBPs5_wJeXtycraidzedzHtLDpLX9a4N5YT1eCC7Y7cWqasEY-p1WX21chRzvh4cZ4hVhrDyvy-FRKNoVaw4jWRHZ5IXmJT7GHy8S9pQIJQFEwVJpB03Nc15ZHxqDCPLI6on" alt="Example of a request in spreadsheet format."><figcaption></figcaption></figure>

## Convert Excel spreadsheet into MARC&#x20;

{% hint style="info" %}
This is mostly an automated process, but if the requester enters information in Additional note, you will need to do some manual editing after this process is done.
{% endhint %}

Open MarcEdit’s Delimited Text Translator (Ctrl+D or Tools—Delimited Text Translator)&#x20;

For Source File, locate the EXCEL spreadsheet by clicking the folder icon. For Output File, select a location for the destination file (\*.mrk) by clicking the folder,  check the UTF-8 Encoded box and click the “Import” button to import the EXCEL file. &#x20;

![](https://lh6.googleusercontent.com/cHPMnbniA2Qc1gckdF63GqrjaGbdvxMGCPq4nyE3Q6Q\_ctRtdvgaOjB84yR4DmpC9Ethk4X3AwAJJK\_415PEu0ZV-fp6nxZKpqb2tKkCFUVKa9eBip5\_KhFgsWXAt4O2NThT\_TxG\_AtptIPQAf8-eUJnTSYBdMdv)

\
Click the “Load Template” button and select “POL creation updated\_2-24-22.mrd”

\[The template is located at:   Google drive –> Alma(RDG)  –> [Brief record/POL creation](https://drive.google.com/drive/u/0/folders/1cxeRXaXnxTnlm8m7aFJrn-X\_SGEx9vtS)]

![](https://lh5.googleusercontent.com/9jzhEmkjYFVRjOge2yTDMRv65fhE0Xi0gOXawO711PyNTFRLNu3pRN-ZEhzE2g75F7oL\_NVvcO\_OQpbcJT3x7KasO6p1dFZDCVL7yz9q7mtbMAX90RxFiIvb0e4HEbUj0TyXUrdOIczPpQeUECcghwdQIuVv31V7)

Note: In the template, all 960 lines are joined into one line 960. See the asterisk next to each 960 line.&#x20;

Click the “Finish” button to complete the conversion.&#x20;

Open the output \*.mrk file in MarcEditor and remove the 1st record, which is from the header of the Excel file.&#x20;

Convert the file into \*.mrc file (File—Compile File into MARC)&#x20;

{% hint style="info" %}
General format of the mrk record:

\=LDR  00000nam a2200000Ia 45e0

\=008  220907s9999\\\\\\\xx\\\\\\\\\\\\\\\\\\\\\\\000\0\und\d

\=020  \\\\$aISBN

\=024  \\\\$aVendor reference number

\=035  \\\\$aOCLC #

\=245  \0$aTitle

\=960  \\\\$aLocation$bPrice (in US$)$dFund code$hVendor code$iReporting code$gQuantity$uInterested&#x20;
{% endhint %}



## Import

When importing, you will need to use the import profiles under "Aquisitions > Import". Use the import profile “Create new orders”.&#x20;

Once the import job is complete, double check the import job report to ensure that everything was loaded correctly. &#x20;

{% hint style="warning" %}
The import profile default holdings location is “stacks'' and item type // policy is Book//regular loan”.   If the item is a media location or other location, and the item type is DVD for example, then we need to manually change them to match with the item ex. grcmed, DVD//DVD
{% endhint %}

## Communicating POL creation

You'll want to create a set << link to creating a set in Alma from the job >> in Alma to share with the requestor. The set name should follow the format: “yyyymmdd\_new\_order(x)” \[ x is the number of the records in the batch], make sure to save the set as a public set so the requestor can see it.&#x20;

It takes about 6 hours for Alma to compile POLs into a PO; once it's available email the itemized file name to the requester.   &#x20;

Update the Google sheet by adding your email address on the “Operator email” column.&#x20;
