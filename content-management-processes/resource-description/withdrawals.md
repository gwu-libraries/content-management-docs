# Withdrawals

{% hint style="warning" %}
This covers a broad overview of what to do with withdrawals. For information on how to perform batch withdrawals, please see [withdrawals.md](batch-processing/withdrawals.md "mention").&#x20;
{% endhint %}

### Monograph Withdrawal: Not the last holding/item

Withdraw only the item noted for discard. No additional changes will need to be made to the bib record or other holding records.&#x20;

### Monograph Withdrawal: Last holding/item

When withdrawing items that will leave no items left on the holdings, and no holdings you are withdrawing the final item; assign a withdrawal date, withdraw the holding and the item(s) and delete the bib record.&#x20;

These bib records will remain accessible through APIs with appropriate access to the Dark Archive and Analytics.&#x20;

After withdrawing all records in Alma, remove DGW holdings from the appropriate records in OCLC. In a few cases, the bibliographic record was in Alma only, and was never loaded to OCLC (most common with Special Collections or the NSA Archive). These records will not contain an 035 with $a (OCoLC).&#x20;

### Serials Withdrawal: Complete holdings

When withdrawing all available issues of a serials title, follow the procedure for removing the last holding/item of a monograph title.&#x20;

### Serials Withdrawal: Partial holdings

When withdrawing a partial collection of serials holdings, follow the procedure for Monograph withdrawal: not the last holding/item.\
\
Update the 866 of the holding record to reflect the remaining holdings.

### Withdraw: Damaged/lost discards

All damaged materials must first go through the damaged book review. The reviewers will review the materials in accordance with WRLC retention policy and decide if it should be replaced or discarded.&#x20;

Due to the way that Alma maintains data, items that are replaced (through the damaged book or lost book workflow), still need to be withdrawn. The holdings for these items do not need to be withdrawn, the item should be marked as “Damaged” or “Lost”, and have a withdrawal date assigned.&#x20;

Adding a replacement copy should follow the added copy workflow.&#x20;
