# Serials Withdrawal (Batch)

## Bound Serials issues

For bound serials volumes with item records in Alma, they cannot be sent to WRLC because another institution has already deposited theirs there.

1. Dawn will send a list of barcodes to Shirley through the Salesforce ticket.
2. Shirley will claim the ticket and process the withdrawn in Alma by pulling the data based on the barcodes and deleting the items or items/Holdings/Bibs/OCLC GW holdings (if it is the last volume).
3. Shirley will run an updated report for the titles that will include the MMS IDs and titles only, upload the report to the Salesforce ticket and update the ticket. If there is anything that needs to check with Dawn, Shirley will update the ticket to let Dawn know and get feedback from Dawn before transfer the ticket to Serials Unit (Qali).
4. Transfer the Salesforce ticket to Qali by re-assigning the ticket’s case owner with above updated report (MMSIds and titles only).
5. Qali will claim the ticket and will update the holdings 866 field or even merge the holdings on the same Bib records to consolidate volumes if the holdings with a same location. Qali will closed the ticket when the job is done.
