# Swank Streaming Video

## Introduction

This policy is a guide to the creation of streaming video records in Alma/Primo provided by SWANK. Main purpose is to document steps to perform but specific MARC fields to be added will also be listed.

## Tracking&#x20;

File is under Admin →[Alma Ongoing Record Loads](https://gwu0.sharepoint.com/:x:/r/sites/20180727030128000/Collaboration%20Items/Admin/Alma%20Ongoing%20Record%20Loads.xlsx?d=wade799fa6af14b9aa212b8853cc91183\&csf=1\&web=1\&e=Sd0pxb)

Check before each new load and update information after each load. Use this to keep track of:

* current service used
* latest title load date
* latest title added
* total number of titles added&#x20;

## Cataloging

### Getting records

{% hint style="info" %}
You will need to login to the Swank website. Please see Matthew Bright for login credentials.&#x20;
{% endhint %}

* Click "Content Manager" Tab
* Order titles list by date  using "License Start" Tab&#x20;
* In Alma check for both the most recent title added before this load and the earliest by date in this load before beginning the load: use an All Titles Keywords search XXX title Swank (to limit search results).
* Choose titles to add using check box
* Under Actions Bar choose "All as a zip file" for exporting titles
* Extract data from zip file

### Record enhancement

* Open mrc file
* Run task: Swank create 957 42 blank
* Open digcampus Excel Spreadsheet.
  * &#x20;Cut and Paste image urls for titles from column E (Poster art link) into corresponding MarcEdit titles 957 fields.&#x20;
* Run Task Edit 957 to add: $9LOCAL suffix
* Save mrk file
* Convert back to MarcEdit mrc file

### Import Records into Alma

Use the "Swank discovery records" import profile.&#x20;

Once load is finished, check to make sure records were corrected and display in discovery.

## Electronic collection management

### Choosing electronic collection

{% hint style="info" %}
Each semester, a new Swank collection is created since all titles are licensed until the same cutoff date.&#x20;
{% endhint %}

* Search under Alma Electronic Collection→ Electronic Collection Name: SWANK&#x20;
* SWANK Motion Pictures, Inc → Edit Collection&#x20;
* Click Additional Tab scroll down to find Services&#x20;
  * Only 1 service is used each semester (deactivation at end of license date is automatic)
  * At end of each semester will need to delete titles from the service currently in use
  * Choose the inactive service for the following semester (ie Activate that one)
  * Add new titles to new service
* Go to Swank Discovery Records Profile→ Inventory Information Tab
* Under Electronic Resource Mapping→ Service&#x20;
  * Type/Change name of service you wish to use (either Full Text or Selected Full Text)

## End-of-semester Changeover

* Search under Alma Electronic Collection→ Electronic Collection Name: SWANK&#x20;
* SWANK Motion Pictures, Inc → Edit Collection&#x20;
* Additional Tab→ Ellipsis of Currently active service → Portfolio List
  * Click All titles box
  * Under Activate/Deactivate choose Deactivate All

{% hint style="info" %}

{% endhint %}

*
