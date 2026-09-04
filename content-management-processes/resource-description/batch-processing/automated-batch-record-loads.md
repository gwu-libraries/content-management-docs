# Automated Batch Record Loads

## Firms, Approvals, A\&Aeportal

Import profiles are set up to run automatically to check Worldshare FTP server for new records and will import them into Alma.

## EBSCO DDA Ebook Record loads

EBSCO autoholdings have been set up with OCLC for the “EBSCOHost PDA Ebooks” collection. MARC records are delivered weekly to OCLC FTP/Worldshare Collection Manager. Alma “EBSCO DDA Pool” import profile automatically downloads MARC records from OCLC FTP weekly. Import profile matches by ISBN to activate CZ portfolios in the “EBSCOhost DDA Pool Ebooks (EBSCOhost Ebooks)” electronic collection. The DDA Pool electronic collection has a service-level public note with language explaining that the title is not owned and could be removed from the collection.

### Manually activating titles with multi-match errors

* Check the import job report in the Electronic portfolios for and "Portfolios which were not activated due to multi matching portfolio from the CZ"
* Download sources (XML) just for the "Portfolios which were not activated due to multi matching portfolio from the CZ"
* Open the XML file
* In Alma, search electronic collections for "Ebscohost DDA" and edit the "EBSCOhost DDA Pool Ebooks (EBSCOhost Ebooks)" electronic collection.
  * Additional>Services>...>Portfolio List
  * \+ Add>Add portfolios from community
  * Change dropdown from "title" to "ISBN" and enter ISBN from XML file
  * Select the correct title from results and click "Activate"
  * Confirm
* Repeat for each title listed in the XML file

### Drop Title Process

* Receive "Drop Title Notification" email from EBSCO periodically
* Wait at least a week before taking action on the email
* In Alma, manually search for each ISBN listed in the email
* Find the matching e-resource title
* Look at the electronic portfolios to find the "EBSCOhost DDA Pool Ebooks (EBSCOhost Ebooks)"
* Choose ...>Delete Portfolio
  * If prompted, select the option to Delete bibliographic record(s)
* Repeat for all titles listed in the email
