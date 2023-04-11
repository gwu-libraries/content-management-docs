# Boundwiths

Boundwiths are multiple titles that are bound together in one volume. These are often multiple volumes of the same periodical, but can be discrete monographic titles as well. The bound volume is often called the container or parent; and the items bound within are referred to as the constituent titles or child titles.&#x20;

## Record check

Check the IZ in Alma for all constituent titles. These records may or may not be linked to the NZ, but they should not ever be linked to the CZ. If a constituent title is missing a record, follow the [.](./ "mention"), without adding in any holdings or items.&#x20;

## Create container record

In Alma’s Metadata Editor, create a new  MARC21 Bibliographic Books record in the IZ. Add the following MARC fields as follows:

\
245 00 \$$a GW boundwith titles associated with barcode \[enter barcode on container here]

774 1\  \$$t \[Title proper from the constituent record without leading article] \$$w \[IZ MMSID]

\
Repeat the 774 fields for as many constituent titles as required.&#x20;

Alma will automatically generate the LDR and 008 fields, the default values are acceptable and do not need to be changed.\
&#x20;

Add inventory records according to [.](./ "mention").



{% hint style="info" %}
Every night, Alma will run the job required to create relationships between the container record and the constituent records. This job uses the 774 \$$w in the container bib to link the container and constituent records together.&#x20;
{% endhint %}



## Editing constituent records

Each one of the constituent records need a LOCAL 591 notes field added. Format as follows:



591 \\\ \$$a Bound with: \[Title of 1st title] -- \[Title of 2nd title] -- \[Title of 3rd title]...&#x20;

\
Exclude title of the volume being added. For example, if you are adding the 591 to the Title of 1st title record, you will omit the Title of 1st title.&#x20;

\
