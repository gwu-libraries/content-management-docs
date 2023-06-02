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

#### Enumeration format

For recording dates/volumes/numbers: Follow the established format for each title; enumeration and frequency of publication are different for different periodicals. Here are examples of possible formats:

* **Single volume, year:** v.1 (1997); v.1 (1997)-v.2 (1998)
* **Volume, number, year:** v.27:no.1 (2003); v.27:no.1 (2003)-no.2 (2003)
* **Volume, number, year, month:** v.17:no.1 (2003:Jan.); v.17:no.1 (2003:Jan.)-v.17:no.2 (2003:Feb.)
* **Volume, number, year, season:** v.15:no.1 (1991:Spr.); v.15:no.1 (1992:Spr.)-v.15:no.2 (1992:Sum.)
* **Volume, number, year, month, day:** v.55:no.26 (2003:July 30); v.55:no.26 (2003:July 30)-v.55:no.27 (2003:Aug. 30); v.55:no.31 (2003:Oct. 03); v.55:no.31 (2003:Oct. 03)-v.55:no.32 (2003:Nov. 03)
* **Number, year:** no.5 (1998); no.5 (1998)-no.52 (1999)
* **Number, year, month:** no.36 (2003:Sep.); no.36 (2003:Sep.)-no.37 (2003:Oct.)
* **Number, year, month, date:** no.1 (1995:Jan. 02); no.2 (1995:Feb. 02)-no.51 (1995:Dec. 18)
* **Year, season:** 2003:Sum.; 2003:Sum.-2003:Fall
* **Year, month:** 2000:Oct.; 2000:Oct.-2000:May
* **Year, month, day:** 1994:Apr. 07; 1999:Apr. 07-1999:May 20



{% hint style="info" %}
When adding months or seasons, use either the three character abbreviation (example: Summer - Sum.; January - Jan.) or the full three or four letter name (May, June, Fall).
{% endhint %}

#### Punctuation format

All holdings should be in one 866 (some legacy data has multiple 866 fields). We use punctuation to make it easier to read holdings statements.

* **Continuous coverage**: Use a single dash "-". Example: no.5 (1998)-no.52 (1999)
* **Coverage is broken**: Use a ",". Example: v.17:no.1 (2003:Jan.)-v.17:no.2 (2003:Feb.), v.22 (2005:May)

