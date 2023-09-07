---
description: >-
  Process for updating 866 holding summary statements when a title has multiple
  volumes.
---

# Updating Holding Summary Statements

### Determine what items are associated with a location and holding

Once items have been moved to their destination holding record, examine the list of items on each holding to determine which volumes/ranges are attached to each holding.

{% hint style="info" %}
This process doesn't need to happen if these items are discards! This is only for items that are moving from one location and holding to a different location and holding.
{% endhint %}

### Edit holding record

Edit each holding record in the Metadata Editor to update the 866, 867, and 868 fields to match which items are actually associated with that holding.

<figure><img src="https://lh4.googleusercontent.com/2F3pda-L7IZXAezhMPrOlNNMv0jYV2RKekW6lq2y0BYcRhUqZc1kW9JPCGXkFA137jpJQ2ioRUVheD6J0DDEO8pDpcc72uuwe1KqtzI7xrgJEIX-PlKmxMKgj3o0zTv01WfVdOL8QAURK07wzLVLP73RtbFufrTvAVXAhB5BDBVL5jXqXFZVRmBv" alt=""><figcaption></figcaption></figure>

The 866 field is usually the only one used for summary holding statements. If there are supplemental issues and indexes, these go in the 867 and 868 fields. Edge cases like these can be referred to RDG.

Enumeration information goes in the $a. $8 is not necessary. Enumeration should include a range as long as there are no missing issues. Separate ranges or single issues with a comma. There should only be one 866 per holding record, so it may be necessary to consolidate multiple 866 fields since our previous practice allowed multiple 866s.

Select "Save and release record" when finished. It is very important to release all records when you are done working on them, as they will otherwise remain locked for future editing. Make sure that no records remain listed in the metadata editor.

<figure><img src="../../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

| MARC Field Tag | Purpose          | Example                               |
| -------------- | ---------------- | ------------------------------------- |
| 866            | Textual holdings | $a v. 1 (1997)-v.2 (1998), v.4 (2000) |
| 867            | Supplementary    | $a Supplement to v. 1 (1997)          |
| 868            | Indexes          | $a Index to v.1 (1997)-v.10 (2007)    |

{% hint style="info" %}
Enumeration format guidelines and examples can be found on the [Volume Numbering](../../reference/volume-numbering.md) page.
{% endhint %}

