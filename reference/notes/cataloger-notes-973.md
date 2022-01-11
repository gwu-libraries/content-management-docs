# Cataloger Notes (973)

A cataloger note should be added as a local field to bib records each time cataloging work is done.

| Subfield | Definition       | Options/Format                                                                                                                                                                                                                                                                               |
| -------- | ---------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| $a       | Action           | <p>New title<br>Updated bib<br>Added copy<br>Added volume</p>                                                                                                                                                                                                                                |
| $b       | Cataloging Level | <p><strong>CC</strong> (nothing added)</p><p><strong>CCE1</strong> (something minor added)</p><p><strong>CCE2</strong> (call # provided, subject headings added, major additions like making a brief YBP record a fully encoded level record)</p><p><strong>ORIG</strong> (all original)</p> |
| $c       | Cataloger        | eg. gwbright                                                                                                                                                                                                                                                                                 |
| $d       | Date             | <p>YYYY-MM-DD<br>eg. 2021-01-16</p>                                                                                                                                                                                                                                                          |

## Examples

Jen Froetschel updated an OCLC record with pagination and correcting a typo in the table of contents note, then imported the record to Alma for a new title:

```
=973 \\$aNew title added$bCCE1$cgwfroetschel$d2022-01-01
```

Matthew Bright updated an existing bib record in Alma for an existing item, changing the call number (no $b is needed because this was just an internal record update):

```
=973 \\$aBib record updated$cgwbright$d2021-11-08
```

