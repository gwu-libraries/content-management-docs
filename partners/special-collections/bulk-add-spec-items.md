# Bulk Add Spec Items

This process is for Special Collections to add multiple item records for boxes to an existing Alma record, using an Excel spreadsheet and an Alma import profile.

Prerequisites:

* An existing Alma bibliographic record that is shared with the Network Zone

Drawbacks:

* Imports the item "description" field but does not import/create item "enumeration D" field

## Process

Use the [scrc\_bulk\_add\_items\_to\_alma\_template](https://gwu.box.com/s/rykr6kamxeo8rg17m1ktz9xq7ttop7pm) template file to create your import file, using one row per item record with the following information:

| Field | Data                                             |
| ----- | ------------------------------------------------ |
| 001   | Network Zone MMS ID (ending 4101)                |
| 245$a | Title (does not have to match the title in Alma) |
| 960$b | Barcode                                          |
| 960$d | Description (eg "Box 1)                          |
| 960$r | Receive date (yyyyMMdd format)                   |

The 001, 245$a, and 906$r fields will be the same for all items on the same bib.

Save the Excel file in .xlsx format.

Import the file in Alma by going to Resources>Import and running the "SCRC Item Bulk Creation" import job.

In addition to the information in the spreadsheet, the following information will be added to all item records created through this process:

* Location: scrc
* Item policy: Non-circulating
* Is magnetic: no
* Item type: Box
