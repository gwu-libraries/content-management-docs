---
description: >-
  This covers the Alma record changes needed when sending items to WRLC. The
  process of selecting items to send, and the physical process of boxing and
  sending items, is not included in these steps.
---

# Sending GRC items to WRLC

{% hint style="warning" %}
Before you start: make sure you know what WRLC location the item needs to go into and for periodicals whether the issues/volumes are already held at WRLC.
{% endhint %}

## Title with only 1 holding record

Use only if all conditions are met:

* [x] Only 1 holding record exists on the bibliographic record

Steps:

* Make sure holding 561 is present and accurate
* Use "Scan in items" in Alma to set the location to the desired WRLC location ("wrlc cgrc", "wrlc sgrc", "wrlc shrp", etc)

![](<../../.gitbook/assets/image (3).png>)

* If there is a temporary location (e.g. "In process"), use "Scan in items" in Alma to restore the item to its new permanent WRLC location

![](<../../.gitbook/assets/image (8).png>)

* If the title has multiple items, check the holding records to see if 866 holding summaries need to be created or edited on any of the holding records (multiple holding records may exist if not all items are going to WRLC)

## If some items are already at WRLC

Use only if all conditions are met:

* [x] There is already a holding record with the specific desired target location at WRLC
* [x] The holding record with the desired location has the correct 561 and 541 collection and donor notes (if applicable) for the items that will be sent to WRLC

Steps:

* Make sure holding 561 is present and accurate
* Relink items to the target holding record. _If prompted, do not delete the old holding record unless there are no 866 fields or other notes that are needed in the original holding record._

![](<../../.gitbook/assets/image (9).png>)

* Update 866 fields if necessary for the old and new holding records
* Use "Scan in items" to set "In transit" status for each item

![](<../../.gitbook/assets/image (2).png>)

## If there are multiple items and all GRC items are going to WRLC

Use only if all conditions are met:

* [x] There is more than 1 holding record attached to the bibliographic record
* [x] All items on any particular holding record are being sent to WRLC

Steps:

* Make sure holding 561 is present and accurate
* Edit holding record for the holding that has all items moving to WRLC
* Change the 852 \$$c to the desired WRLC location ("wrlc cgrc", "wrlc sgrc", "wrlc shrp", etc)
* Update 866 fields in the holding record if necessary
* Repeat for any additional holding records on the title that are also moving to WRLC
* Use "Scan in items" to set "In transit" status for each item

## More complex cases/everything else

This method can be used for everything, but is best used only when one of the above doesn't apply.

Steps:

* Edit holding record for the holding that has one or more items moving to WRLC
* Make sure holding 561 is present and accurate
* Duplicate the holding record
* On the new record, change the 852 \$$c to the desired WRLC location ("wrlc cgrc", "wrlc sgrc", "wrlc shrp", etc)
* Relink item records for items going to WRLC to the new holding record. _If prompted, do not delete the old holding record unless there are no 866 fields or other notes that are needed in the original holding record._
* Update 866 fields in both the old and new holding records if necessary/desired
* Repeat for any additional holding records on the title that also have items moving to WRLC
* Use "Scan in items" to set "In transit" status for each item

{% hint style="info" %}
Dummy holding and item records are no longer necessary. It is appropriate to have the holding record with WRLC items unsuppressed, allowing patrons to directly request circulating items and see what non-circulating items are available.
{% endhint %}

## Problems

If you have items that don't work with any of the above, or you aren't sure, please contact [rdg@gwu.edu](mailto:rdg@gwu.edu) for assistance.
