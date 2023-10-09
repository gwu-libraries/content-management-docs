# Serials Binding (LibOps steps)

{% hint style="info" %}
This is part of the overall [Serials Binding](../../reference/workflow-overviews/serials-binding-overview.md) workflow
{% endhint %}

### Step 1: Building Operations and Media Reserves Supervisor selects title to be bound <a href="#docs-internal-guid-a2fc3123-7fff-f71f-0080-cf3084dcc7f0" id="docs-internal-guid-a2fc3123-7fff-f71f-0080-cf3084dcc7f0"></a>

### Step 2: Prepare bindable units

Building Operations and Media Reserves Supervisor and Library Operations Associate prepare bindable units

{% hint style="warning" %}
We still need to decide what to do with incomplete binding units
{% endhint %}

### Step 3: Check to see if volumes should be discarded or sent to WRLC

Once binding units have been identified, check the ISSN into the input box on the WRLC Shared Collection Facility (SCF) link provided below:

[https://grima.wrlc.org/Analytics/ia\_journal\_lookup.php?ISSN=](https://grima.wrlc.org/Analytics/ia\_journal\_lookup.php?ISSN=)

<figure><img src="https://lh5.googleusercontent.com/MNCgwl_HhqC_sNN3fHUQUatqzw3v3vYinZJDV7_R5NXUY0dQsE3ibITLdG0UdB50DLEJCSEtPawhknsPWPUsm0-REp3BeD87sdflQcYj203AUUSALSH8suhZNR_--IRwNX8y-z_aYxW3iWLq_BGhZzU" alt=""><figcaption><p>WRLC Shared Collection Facility serial holdings lookup tool</p></figcaption></figure>

* If bindable unit is at WRLC
  * If unbound issues have individual item records in Alma (because of predictive patterns), send RDG list of barcodes to be withdrawn
  * Edit holding record 866 to remove issues being discarded
  * Physically discard issues
* If volume is not at WRLC, check for online access ([Access Hierarchy checklist](https://docs.google.com/document/d/1p0ZalNnnjoU9Je9i8wmU44YY1mAM2FOOMzpjR3KJUMI/edit)), to see if the issue is in Hathitrust or JSTOR. When in doubt, consult with Collection Development librarians.
  * If volume is in JSTOR (or other repository as agreed upon by Collection Strategist and Building Operations and Media Reserves Supervisor)
    * If unbound issues have individual item records in Alma (because of predictive patterns), send RDG list of barcodes to be withdrawn
    * Edit holding record 866 to remove issues being discarded
    * Physically discard issues
* If volume is not at WRLC AND is not in approved e-resource repository, continue to the next step to prepare issues for binding

### Step 4: Preliminary Bindery Prep

Library Operations Associate prepare issues for binding

* Fill out binding slip (including title, enum, chron) with as much information is needed for the title.&#x20;
  * DO fill out holding # (for when slip goes to Qali)
  * Don’t need “numbers”
  * Don’t need “months”
* Attach barcode to slip
* If unbound issues have individual item records in Alma (because of predictive patterns):
  * Select the item records of the issues that will be bound
  * Choose Manage Selected>Bind Items
  * Confirm items
  * Generate work order: Acquisition technical services, then click “Create And Edit”
  * Edit the item record including material type (bound issue), blank item policy, Enum and Chron information, and generating description, set permanent location to “wrlc shrp”
    * See [guidance for Enum, Chron, and Description field usage](../../reference/volume-numbering.md)
* If unbound issues do not have item records in Alma:
  * Create “wrlc shrp” holding record if one does not already exist
    * Optional: add/update 866 field
  * Under the “wrlc shrp” holding record, create item record including barcode, material type (bound issue), blank item policy, Enum and Chron information, and generate description
    * See [guidance for Enum, Chron, and Description field usage](../../reference/volume-numbering.md)
    * After saving the item record, edit it to set process type to “Acquisition Technical Services” and select At: “gelman Content Management”
* Deliver physical issues and binding slips to Monograph Acquisitions

{% hint style="info" %}
This process continues with [steps for Monograph Acquisitions](../../content-management-processes/bindery/serials-binding-monoacq-steps.md)
{% endhint %}
