---
description: >-
  This covers the Art Approval, FIRM order, Horrworth records, and A&AePortal
  records.
---

# WorldShare Management Services

### Downloading

* Login to [WMS](https://gw.share.worldcat.org/wms/cmnd/), and navigate to the "Downloads" tab.&#x20;
* Download batch MARC records: Approval, FIRM or Horrworth or AAePortal (new or update) MARC records.&#x20;
* Convert the\*.mrc file to \*.mrk file and apply MarcEdit task to each individual \*.mrk file

### ACQ Approvals, Firm, and Horrworth

In MarcEdit run the following tasks: (task list available in SharePoint)

* Delete 961 field
* Delete 938 field
* buildnewfield :=961  \\\\$b{960$b}$d{960$d}$f{960$f}$g{960$g}$m{852$b}$n{852$c}
* Delete 960 field
* Delete 852 field
* Copy 961 field to 960 field - delete source field
* Copy 960 $dGHORRWORTH field to 971 field
* Bulidnewfield : =971 2$a{971$d} - replace existing field
* Editfield 971 $aGHORRWORTH - replace $aJohn Horrworth Children's Literature Collection. $9local
