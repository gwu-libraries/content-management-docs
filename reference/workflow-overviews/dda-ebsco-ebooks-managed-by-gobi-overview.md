# DDA EBSCO Ebooks managed by GOBI Overview

* [Record loads (Resource Description Group)](../../content-management-processes/resource-description/batch-processing/automated-batch-record-loads.md)
  * EBSCO autoholdings set up with OCLC for the “EBSCOHost PDA Ebooks” collection
  * Records are delivered weekly to OCLC FTP/Worldshare Collection Manager
  * Alma “EBSCO DDA Pool” import profile automatically downloads MARC records from OCLC FTP weekly
  * Import profile matches by ISBN to activate CZ portfolios in the “EBSCOhost DDA Pool Ebooks (EBSCOhost Ebooks)” electronic collection
* [Purchases (Monograph Acquisitions)](../../content-management-processes/acquisitions/ebsco-dda-ebook-triggered-purchase.md)
  * GOBI sends purchase notification
  * MonoAcq moves the electronic portfolio from the “EBSCOhost DDA Pool Ebooks (EBSCOhost Ebooks)” electronic collection to the “EBSCOhost Ebooks” electronic collection
  * MonoAcq creates POL
* Maintenance (TBD)
  * Periodically link standalone portfolios in “EBSCOhost Ebooks” electronic collection to CZ
  * Remove DDA Pool records for titles that have been removed from the pool (TBD)
