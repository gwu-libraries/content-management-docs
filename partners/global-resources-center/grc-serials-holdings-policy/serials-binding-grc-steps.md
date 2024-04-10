# Serials Binding (GRC steps)

{% hint style="info" %}
This is part of the overall [Serials Binding](../../../reference/workflow-overviews/serials-binding-overview.md) workflow
{% endhint %}

### Step 1: Director of Global Resources selects title to be bound <a href="#docs-internal-guid-a2fc3123-7fff-f71f-0080-cf3084dcc7f0" id="docs-internal-guid-a2fc3123-7fff-f71f-0080-cf3084dcc7f0"></a>

### Step 2: Prepare bindable units

GRC staff prepare bindable units

### Step 3: Preliminary Bindery Prep

GRC staff prepare issues for binding

* Fill out binding slip (including title, enum, chron) with as much information is needed for the title.&#x20;
  * Include holding ID #
  * Enumeration and Chronology is only needed with enough specificity to cover the full range of the bindable unit (For example, if v.2 no.1-4 are being bound, and there are only 4 issues per year, then only "v.2" is needed, "no.1-4" is not necessary; but if there are 8 issues per year then "v.2 no.1-4" is necessary because v.2 by itself does not indicate that only part of the volume is included in that bindable unit.)
* Attach barcode to slip
* Create item record in Alma:
  * Find the holding record for the issues being bound (the location will not change)
    * Optional: add/correct 866 field if needed
  * Under the holding record, create item record including barcode, material type (bound issue), blank item policy, Enum and Chron information, and generate description
    * See [guidance for Enum, Chron, and Description field usage](../../../reference/volume-numbering.md)
    * After saving the item record, edit it to set process type to “Acquisition Technical Services” and select At: “gelman Content Management”
* Deliver physical issues and binding slips to Monograph Acquisitions

{% hint style="info" %}
This process continues with [steps for Monograph Acquisitions](../../../content-management-processes/bindery/serials-binding-monoacq-steps.md)
{% endhint %}
