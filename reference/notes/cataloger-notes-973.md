# Cataloger Notes (973)

A cataloger note should be added as a local field to bib records each time cataloging work is done.

<table><thead><tr><th width="150">Subfield</th><th width="156.26277372262774">Definition</th><th>Options/Format</th></tr></thead><tbody><tr><td>$a</td><td>Action</td><td>New title added<br>Bib record updated<br>Added copy<br>Added volume</td></tr><tr><td>$b</td><td>Cataloging Level</td><td><p><strong>CC</strong> (nothing added)</p><p><strong>CCE1</strong> (something minor added)</p><p><strong>CCE2</strong> (call # provided, subject headings added, major additions like making a brief YBP record a fully encoded level record)</p><p><strong>ORIG</strong> (all original, including records that were derived from another record)</p></td></tr><tr><td>$c</td><td>Cataloger</td><td>eg. gwbright</td></tr><tr><td>$d</td><td>Date</td><td>YYYY-MM-DD<br>eg. 2021-01-16</td></tr><tr><td>$9</td><td>local designation</td><td>local or LOCAL*</td></tr></tbody></table>

\*NOTE: If cataloging in Alma's Metadata Editor, use "Add local extension" under the "Editing Actions" menu. The key command shortcut is CTRL + L. Do not add \$$9 LOCAL, it will cause issues in the NZ record.&#x20;

## Examples

Jen Froetschel updated an OCLC record with pagination and correcting a typo in the table of contents note, then imported the record to Alma for a new title:

```
=973 \\$aNew title added$bCCE1$cgwfroetschel$d2022-01-01$9LOCAL
```

Matthew Bright updated an existing bib record in Alma for an existing item, changing the call number (no $b is needed because this was just an internal record update):

```
=973 \\$aBib record updated$cgwbright$d2021-11-08$9LOCAL
```

