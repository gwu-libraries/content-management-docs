# Withdrawals

<< We need to add how we get withdrawals, including where they are on the shelves in 104. Or if they're just emailed/sent through Salesforce >>&#x20;



### Alma Analytics

Use the list of barcodes that were either provided to you or that you scanned to run an analysis in Alma Analytics for items' retention information, other ID numbers for running jobs, etc.

{% hint style="success" %}
Save your analysis to save work later in the process!&#x20;
{% endhint %}

It's recommended to also pull the following fields:

* MMSID
* Title
* OCLC no.
* Holding ID
* Summary Holding
* Location code
* Item ID
* Barcode
* Enum A
* Has Committed to Retain
* Retention note

{% hint style="danger" %}
If there is any item with a retention note and the “Has Committed To Retain” value = Yes, then remove the item from the withdrawn list and notify the project manager to not discard the item.&#x20;
{% endhint %}



### Running Alma Jobs: Add weeding date and withdraw

Create a "Physical Items" set, then run the Alma “Change Physical Items Information” job to batch add today’s date in the item records as “Weeding date”.

<figure><img src="../../../.gitbook/assets/weeding date.png" alt="Weeding date box is checked and the date is entered into the field."><figcaption><p>Don't forget to check the box. Changes won't happen otherwise.</p></figcaption></figure>

After the weeding date has been added, run Alma “Withdraw Physical items” job to batch withdraw items or item/holdings or item/holdings/bib records. Select the option to "Delete holdings, delete bibliographic records that have no other holdings".&#x20;

When the job is complete, check the job report to make sure that there were no errors. Resolve errors as necessary.&#x20;

### Update holdings in Alma

The day after withdrawing items--Filtering on Holding Id--update the report previously run in Alma Analytics to see if there is any active item(s) attached to the same holdings, then to manually examine if the holdings 866 field need to be updated for the holdings with multiple items/volumes.

Filters to apply:

* Holding Lifecycle is equal to / is in Active
* AND  Weeding Date is null
* AND  Lifecycle is equal to / is in Active
* AND  Holding ID is equal to / is in \[insert all Holding Ids from withdrawn items]

If there are any active item(s)/volume(s) remaining on the same holdings of withdrawn item/volumes, manually update the holdings 866 field.&#x20;

The following example is shows that the v.2 has been deleted but the v.1 is still on the same holdings, so the “v.2 on the 866 field (Summary Holding)” needs to be removed to update match the current holdings:

<figure><img src="https://lh6.googleusercontent.com/qL8rm65sk5df0o7ZOifEf-SlS_tgX6ZiUFgZYb_xIaYQxj1Ctay_VE3r2-fTbFJeOcl9CoRiFoO7PextiptTBYFr1gUHBRAvSp_2-TYgp-FEYb_CbNkySXNOWokf5DQCpnOu8WOhcG3paDXCBXFXoBr-uB1RTdDt" alt="Alma analytics analysis shows that there is only volume 1 still in repository, but the holding statement includes volume 2. "><figcaption><p>Analytics analysis display</p></figcaption></figure>

<figure><img src="https://lh4.googleusercontent.com/ygbiSQcyqKO9Mw1_6PtnvqN8TumcEDWYTqyR32HNG7kEeG7xS6ZtAMzrOcdp1UVhsJHwVuLCcJMc_OgOfAr186z2KQ8JaloQMOxWehAzBOuckCIDxIXIdWdzPRrA9rOkbS_PA_L0U7OKwcjH2xq-TDukMhH7X6ks" alt="Alma holding record has an updated 8 66 field showing only volume 1 in holdings"><figcaption><p>The updated 866, no longer showing volume 2. </p></figcaption></figure>

### Update OCLC holdings

After withdrawals and holdings have been updated in Alma, holdings must be removed from OCLC.&#x20;

In Alma Analytics, using the analysis you created, filter by the unique MMS Ids from, with a Bibliographic Lifecycle equal to/ is in Deleted.

<figure><img src="https://lh6.googleusercontent.com/2p2X0bmKh_zmxpFa5sC8oCXd2chb8_WU1s3kv-Risqk7hfyQdFEhjciyzPpSDKEJJL9MiLQGngkZ6S_UuIUCzMq0N59SecDK2BhPR6rlrlli5ufKDdHKocbwAx5_uNrIEd2zs5w3TD6yyTGagED73G6bBuaW8uEh" alt="Alma analytics analysis filtering bibliographic lifecycle is equal to / is in deleted AND M M S I D is equal to / is in [m m s i d numbers from example]"><figcaption></figcaption></figure>

Copy the OCLC number of the records with value “Deleted” in Bibliographic lifecycle column and paste them into a text document without a header and save the text file.&#x20;



In Connexion Client:

1. Click on the “Batch” tab
2. Holdings by OCLC Number
3. Browse
4. import the above OCLC number text file to the window as below (Do not delete original OCLC number text file after loading them)
5. check the “Delete Holdings”&#x20;
6. Click “OK” to delete the GW holdings

<figure><img src="https://lh4.googleusercontent.com/WindgPuLgbHb__saPoup53NDD8Cel-RRK7mIzbWB3-gJmvNVsZNOzFonU7LqDcY4hfY8z5slDrhUM-6bce8h5EoB7VWjNaKj-H3f4nwt8ey2H6LYLxVs98ZEmQ_cl83RufjXe9vQNUGwhjqxslJHVf7C01eJ45_f" alt="OCLC Connexion batch update window, highlighting the O C L C numbers have been imported from the file, and &#x22;delete holdings&#x22; has been selected."><figcaption></figcaption></figure>

Updating holding in Connexion will ensure OCLC WorldShare is updated and reflects GWU holdings.    &#x20;



### Monograph Withdrawal: Not the last holding/item

Withdraw only the item noted for discard. No additional changes will need to be made to the bib record or other holding records.&#x20;

### Monograph Withdrawal: Last holding/item

When withdrawing items that will leave no items left on the holdings, and no holdings you are withdrawing the final item; assign a withdrawal date, withdraw the holding and the item(s) and delete the bib record.&#x20;

These bib records will remain accessible through APIs with appropriate access to the Dark Archive and Analytics.&#x20;

After withdrawing all records in Alma, remove DGW holdings from the appropriate records in OCLC. In a few cases, the bibliographic record was in Alma only, and was never loaded to OCLC (most common with Special Collections or the NSA Archive). These records will not contain an 035 with $a (OCoLC).&#x20;

### Serials Withdrawal: Complete holdings

When withdrawing all available issues of a serials title, follow the procedure for removing the last holding/item of a monograph title.&#x20;

### Serials Withdrawal: Partial holdings

When withdrawing a partial collection of serials holdings, follow the procedure for Monograph withdrawal: not the last holding/item.\
\
Update the 866 of the holding record to reflect the remaining holdings.

### Withdraw: Damaged/lost discards

All damaged materials must first go through the damaged book review. The reviewers will review the materials in accordance with WRLC retention policy and decide if it should be replaced or discarded.&#x20;

Due to the way that Alma maintains data, items that are replaced (through the damaged book or lost book workflow), still need to be withdrawn. The holdings for these items do not need to be withdrawn, the item should be marked as “Damaged” or “Lost”, and have a withdrawal date assigned.&#x20;

Adding a replacement copy should follow the added copy workflow.&#x20;

\


### Finish

Notify the withdrawal project manager through the Salesforce ticket or email when the batch deletion process is completed so they can physically discard these items.

\


