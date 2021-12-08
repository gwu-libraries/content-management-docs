# Work orders

In order to ensure consistency in how Alma statuses are applied in the library and correctly updated, these documents outline the required setup and steps for managing statuses. In general, when items are received by a department they should be scanned in, either to set a status to keep the item out of place or to remove the “In Transit” status for shelving.

\


In Content Management, all staff should have their location in Alma set to “gelman Content Management”. This will allow them to scan items into the department, set Content Management statuses, and “Manage In Process Items” to view everything in the department.

\


Required Alma roles:

* Receiving Operator (gelman Content Management)
* Work Order Operator

\


![](https://lh3.googleusercontent.com/DroTXlbieR15n7hIfzPrDkaVch4BEzJQ-6jJ395tzvIchX9fwnzGhzZnqNKQ0Ga\_vdFv48Go8H-eceB-0b4fCnLxErTiUOTxhYv1dRin5TuQ\_eDMCkVmJwvg\_hk4UvzRmIKk4YbW)

\


## Work Order Types, Departments, Statuses

The Work Order Type, also referred to in Alma as Process Type, is a top-level category of the work to be performed. The Work Order Type will have one or more departments associated with it, and usually has statuses that are subsidiary to it.

\


At GW we are using the “Content Management” Work Order Type for everything that happens in Content Management, with specific statuses for cataloging, bindery, processing, etc. This Work Order Type is associated with the “gelman Content Management” Work Order Department. Items in the following Alma libraries can be assigned to the “gelman Content Management” department:

* Eckles Library
* Gelman Library
* Virginia Science & Technology Campus Library

\


Work Order Types can be assigned to items by anyone in Alma, but Work Order Statuses can only be assigned by people in the managing department, either through “Manage In Process Items” or “Scan In Items.”

\


When work is complete, an item should be set to “Done,” placing it “In Transit” until it is scanned in at its destination (eg Circ, Spec, etc.)

\


Ultimately, with a few exceptions, everything that comes through the Content Management area should be scanned into the department and assigned a work order status, and then be scanned “done” before it leaves Content Management.

\


## Working with Statuses

### Assigning an Initial Status

#### When Receiving

Be sure to check the “Keep in Department” checkbox on the Alma Receive screen. This allows you to choose the status that will be assigned when the item is received, and keeps the item from being set to “in transit” upon receipt.

![](https://lh3.googleusercontent.com/RPEzkryU1N6\_1e1r3VJmBNGIMtD0Q-\_iF2xQq4Ocyk8npeZ5bAct9hsdOJJjhTSM9wi2AmJKUXoTFS9POuzYNz2i9Wh87Qge33TKigVJTpkJp0MfsKjOkx88enRiQA\_uYCNxQz4P)

\


#### Using “Scan In Items”

Set the status from the dropdown in the Scan In Items screen (with “Done” set to “No”), then scan the barcode.

![](https://lh4.googleusercontent.com/uMiVqZHRgblUlRTXUVtBFUf53B-Gbyeo9m8MCWyygtdSiYhxOPlZ3IAP1bW0cKsORAXQXtJMu2UAcLfrvNccr9LyGrGGVHaZzwJfkidj4DU0O0UX\_CjIVdWbsT0l8bpCKJqMbR3O)

\


### Changing a Status

#### Using “Manage In Process Items”

Select the item in the list, then “Change Status” and choose the desired status.

![](https://lh6.googleusercontent.com/329lL4KII6\_F2qu87pPzLbp0smaE5dnFmIn23qPfKMBJFcNE80G4HPWo\_vNOMd8\_hFb3uq89Ghhf5MGdYyJhZKk6Py45uYLLy0U3CoSgMIBmqQKDLWEFFcx5b0GXx-FiMr\_lll97)

\


#### Using “Scan In Items”

This is done in exactly the same way as assigning an initial status, above.

\


### Placing an Item “In Transit”

#### Using “Manage In Process Items”

Either select the item in the list, then click “Done” at the top of the list; or, click the “...” button for the item and select “Done.”

![](https://lh5.googleusercontent.com/HdlpE1VbRKIGaoDK-UxrJk8-icergcnVue07dbpxrUwbBAvDhCuAW6Vdv75T4KFjoDlTpNCKVMPneQc0LpxDjfzo\_0APP1T88c5NV1-51gSeGaL70lbGOkTtckP814hbNRiIY\_lo)

\


#### Using “Scan In Items”

Select the “Done” value of “Yes” and scan the barcode. When “Done” is set to “Yes,” the “Set Status To” field is ignored.

![](https://lh5.googleusercontent.com/2HlvFhf4-aYUg3rtehDMXXuNInralnOuJFHs2X3ejgezMkL4l4WDVVULCokCUkM8caT8bSVuNf4aja\_nbEJmsTSUK1C0hqoqT8FCWDXzQaMZ1\_7sD1F26Xz6cvqB45Nu0C\_TrqxM)

\


### Completely Removing a Status to Make Item “Available”

When an item is set to “Done,” the work order is removed, and the item status is set to “In Transit” until it is scanned in at its destination (or the department managing the next request, if there is another request on the item.) If you want to place an item directly on the shelf in the stacks, or if the item is going to a partner like the Textile Museum that doesn’t scan in items to set them in place, the item needs to show as “Available” and not be “In Transit.” Be careful using these options, as they can affect other pending requests on the item. Two of the easiest ways to do this are outlined here:

#### Toggle Missing Status

While the item status is “In Transit,” set the status to “Missing” by using “Toggle Missing Status” in a list of items. Then, “Toggle Missing Status” again to remove the “Missing” status, leaving the item showing “Item in place.”

#### Assign and Remove a “Process Type” in the Item Record

Select “Acquisition technical services” in the “Process type” dropdown in the item editor.

![](https://lh5.googleusercontent.com/Dy\_3ikqQiXDZ13ZVkjqAA2dVQqNb9bkOWfpxZ71CvRc13hA12jt5tI9A8vB7RnUq3OgJkTghG6\_9IGOGkRJCOlvaEXxsUNoEZOkXphzYJKoeXGSNJXPMrxqs1ZsF6rsjB9qAhzpE)

Save the item.

Then, edit the item again, select the blank option in the “Process type” dropdown, and save the item.

![](https://lh6.googleusercontent.com/tFtWhOK3\_dRE5q9dRHOjvW7GssTnBu2Of2cM54zVq4PfRmYAJEHD0ywzrcGM7Q87HAdEzYYURwH36A8ySqptmh6PZvzIGcQ4rhvXLeek8KgqjkCR4G3nWxSqAS9KoRLIVkeI3eLT)

The item should now show as “Item in place.”

\


If the item is already in a work order, you can skip the first step and just set the process type to blank to remove the work order and force the item to be in place.

## Shelves and Statuses

The shelves in 103 are grouped by the type of work to be performed and the department performing the work. The Alma statuses are less specific than the labeled shelves. The table below lists the shelves, associated statuses, and flags (if used).

\
\


| SHELF                                                                             | STATUS                                | FLAG        |
| --------------------------------------------------------------------------------- | ------------------------------------- | ----------- |
| Incoming                                                                          | <p><br></p>                           | <p><br></p> |
| Current Periodicals                                                               | <p><br></p>                           | <p><br></p> |
| Received by GRC                                                                   | <p><br></p>                           | <p><br></p> |
| Received Elsewhere                                                                | <p><br></p>                           | <p><br></p> |
| Damaged - CDL Review                                                              | <p><br></p>                           | <p><br></p> |
| Damaged - Retention                                                               | <p><br></p>                           | <p><br></p> |
| Problem Items - Stacks                                                            | <p><br></p>                           | <p><br></p> |
| Problem Items - GRC                                                               | <p><br></p>                           | <p><br></p> |
| Problem Items - Spec                                                              | <p><br></p>                           | <p><br></p> |
| Problem Items - VSTC                                                              | <p><br></p>                           | <p><br></p> |
| Problem Items - Eckles                                                            | <p><br></p>                           | <p><br></p> |
| Problem Items - Work Order Requests                                               | <p><br></p>                           | <p><br></p> |
| Patron Replacements                                                               | <p><br></p>                           | <p><br></p> |
| <p>Needs Attention</p><p>(unknown status; not sure where to place item; etc.)</p> | <p><br></p>                           | <p><br></p> |
| Receiving                                                                         | <p><br></p>                           | <p><br></p> |
| Regular Items Awaiting Receiving                                                  | <p><br></p>                           | <p><br></p> |
| GRC - CDC                                                                         | <p><br></p>                           | <p><br></p> |
| GRC - JRC                                                                         | <p><br></p>                           | <p><br></p> |
| GRC - KRC                                                                         | <p><br></p>                           | <p><br></p> |
| GRC - MENA                                                                        | <p><br></p>                           | <p><br></p> |
| GRC - REECE                                                                       | <p><br></p>                           | <p><br></p> |
| GRC - TRC                                                                         | <p><br></p>                           | <p><br></p> |
| Other GRC                                                                         | <p><br></p>                           | <p><br></p> |
| Other Special Items Awaiting Receiving                                            | <p><br></p>                           | <p><br></p> |
| Review                                                                            | <p><br></p>                           | <p><br></p> |
| For CDL Review                                                                    | Damaged - CDL Review                  | <p><br></p> |
| CDL Replace                                                                       | Damaged - CDL Review                  | <p><br></p> |
| CDL Rebind                                                                        | Damaged - CDL Review                  | <p><br></p> |
| CDL Withdraw                                                                      | Damaged - CDL Review                  | <p><br></p> |
| Damaged                                                                           | <p><br></p>                           | <p><br></p> |
| Damaged - Replace                                                                 | Damaged - Replace                     | <p><br></p> |
| Damaged - Bindery                                                                 | Damaged - Bindery                     | <p><br></p> |
| Ready for Bindery                                                                 | Sent to Bindery                       | <p><br></p> |
| Cataloging                                                                        | <p><br></p>                           | <p><br></p> |
| Rush                                                                              | Cataloging                            | <p><br></p> |
| Firms                                                                             | Cataloging                            | <p><br></p> |
| Approvals                                                                         | Cataloging                            | <p><br></p> |
| Eckles                                                                            | Cataloging                            | <p><br></p> |
| Spec                                                                              | Cataloging                            | <p><br></p> |
| Stacks Gifts - Not in Alma                                                        | <p><br></p>                           | <p><br></p> |
| VSTC - Not in Alma                                                                | <p><br></p>                           | <p><br></p> |
| Eckles - Not in Alma                                                              | <p><br></p>                           | <p><br></p> |
| Spec - Not in Alma                                                                | <p><br></p>                           | <p><br></p> |
| Textile Museum - Not in Alma                                                      | <p><br></p>                           | <p><br></p> |
| GRC - CDC                                                                         | Cataloging                            | <p><br></p> |
| GRC - JRC                                                                         | Cataloging                            | <p><br></p> |
| GRC - KRC                                                                         | Cataloging                            | <p><br></p> |
| GRC - MENA                                                                        | Cataloging                            | <p><br></p> |
| GRC - REECE                                                                       | Cataloging                            | <p><br></p> |
| GRC - TRC                                                                         | Cataloging                            | <p><br></p> |
| Other GRC                                                                         | Cataloging                            | <p><br></p> |
| Problem Items                                                                     | <p><br></p>                           | <p><br></p> |
| Stacks                                                                            | Cataloging Problem                    | <p><br></p> |
| WRLC-SCF                                                                          | Cataloging Problem                    | <p><br></p> |
| GRC                                                                               | Cataloging Problem                    | <p><br></p> |
| Spec                                                                              | Cataloging Problem                    | <p><br></p> |
| VSTC                                                                              | Cataloging Problem                    | <p><br></p> |
| Not in Alma                                                                       | <p><br></p>                           | <p><br></p> |
| Withdraw                                                                          | <p><br></p>                           | <p><br></p> |
| Withdraw                                                                          | Withdraw                              | <p><br></p> |
| Patron Replacements                                                               | <p><br></p>                           | <p><br></p> |
| Patron Replacements                                                               | Patron Replacements                   | <p><br></p> |
| Physical Processing                                                               | <p><br></p>                           | <p><br></p> |
| Rush                                                                              | Physical Processing                   | <p><br></p> |
| Stacks                                                                            | Physical Processing                   | <p><br></p> |
| WRLC-SCF Return                                                                   | Physical Processing                   | <p><br></p> |
| WRLC-SCF Move                                                                     | Physical Processing                   | <p><br></p> |
| GRC                                                                               | Physical Processing                   | <p><br></p> |
| Spec                                                                              | Physical Processing                   | <p><br></p> |
| VSTC                                                                              | Physical Processing                   | <p><br></p> |
| Eckles                                                                            | Physical Processing                   | <p><br></p> |
| Label/Relabel Only                                                                | Physical Processing                   | <p><br></p> |
| Complete - Rush                                                                   | Physical Processing                   | <p><br></p> |
| Complete - Stacks                                                                 | Physical Processing                   | <p><br></p> |
| Complete - WRLC-SCF Return                                                        | Physical Processing                   | <p><br></p> |
| Complete - WRLC-SCF Move                                                          | Physical Processing                   | <p><br></p> |
| Complete - GRC                                                                    | Physical Processing                   | <p><br></p> |
| Complete - Spec                                                                   | Physical Processing                   | <p><br></p> |
| Complete - VSTC                                                                   | Physical Processing                   | <p><br></p> |
| Complete - Eckles                                                                 | Physical Processing                   | <p><br></p> |
| Complete - Label/Relabel Only                                                     | Physical Processing                   | <p><br></p> |
| Ready                                                                             | <p><br></p>                           | <p><br></p> |
| In Transit - Rush                                                                 | In Transit                            | <p><br></p> |
| In Transit - Stacks                                                               | In Transit                            | <p><br></p> |
| In Transit - WRLC-SCF Return                                                      | In Transit                            | <p><br></p> |
| In Transit - WRLC-SCF Move                                                        | In Transit                            | <p><br></p> |
| In Transit - GRC                                                                  | In Transit                            | <p><br></p> |
| In Transit - Spec                                                                 | In Transit                            | <p><br></p> |
| In Transit - VSTC                                                                 | In Transit                            | <p><br></p> |
| In Transit - Eckles                                                               | In Transit                            | <p><br></p> |
| Ready - Textile Museum                                                            | None (should show as “Item In Place”) | <p><br></p> |

\
\
