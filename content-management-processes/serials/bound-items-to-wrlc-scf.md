# Bound items to WRLC SCF

## Item location to WRLC SHRP

After serials are bound, they are sent offsite to the SCF. All items sent to the SCF are part of the shared periodical program in WRLC, and will receive the location "WRLC SHRP".&#x20;

### Analytics

In analytics, using the barcode list from the SalesForce ticket (the ticket is created when the barcode list is emailed to rdg@email.gwu.edu), get the ITEM IDs.&#x20;

Create a set using the Item IDs.

Run the Alma job "Change physical items information", and change the permanent location to wrlc shrp and set all temporary location information to no and clear the data.&#x20;

<figure><img src="https://lh5.googleusercontent.com/fA-QtRb41-RSGYlRsLF8ctg9ARA0LzLEmfFNc5pnY5ynzLq7eLm6xgZlu9Ad4yAUZ8x5rJwcpPUO01srj6wb-G-bTkdzEbltKRqFG0LvtClT4Oo6elK_Llv3KJCadnfTwaXIK_bxS7rc132o69_f_qeC-d0Lzelw" alt=""><figcaption></figcaption></figure>

After the job is complete, check the job report to make sure there were no errors. And double check in Analytics the next day.&#x20;

## Update 866

After the location has been updated, the 866 information will need to be updated.&#x20;
