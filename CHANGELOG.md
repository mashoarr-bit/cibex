# Release Notes

## Version 1.1 (November 2026)

* Fixes the email warning: Gmail and some other mail services reported a virus in version 1.0. There was none. Version 1.0 kept the PDF reader inside the file in a packed form that is unpacked when the page opens, and mail scanners treat that pattern as suspicious. Version 1.1 carries the same PDF reader as ordinary page code, so there is nothing packed or hidden in the file.
* Smaller file: about 2.1 MB instead of 2.8 MB.
* Nothing else changed. Tested on more than 200 CIB reports: every contract, every month of history and every check is the same as in version 1.0.
* Very large reports (thousands of pages) can keep the page busy for a little longer while they are read.

File: CIBEX_v1.1.html
SHA 256: 9f2af39c1812e5acd820184facef61753d96bc3e6a7cd14fcac9d74192b1fae0

To check your copy on Windows, open Command Prompt in the folder with the file and run:

    certutil -hashfile CIBEX_v1.1.html SHA256

## Version 1.0 (November 2026)

First public release.

* Assessment: current classification as borrower and guarantor, late payment by year, and Yes or No checks with contract codes (24 for borrower and co borrower, 16 for guarantor).
* Contracts: every facility with a 24 month repayment strip and full monthly history.
* Analytics: late payment recency, limit use trend over 24 months, and a DBR calculator.
* Summary and Data Checks tabs.
* Excel export (six sheets), one page Print Summary and full HTML export.
* Several CIB reports for one loan.
* Light and dark mode.
* Fully offline: nothing is uploaded.

File: CIBEX_v1.0.html
SHA 256: 63de4a68b17009906562aa7f63d9e1c34850d92409003e63187c24d26bccb09b

To check your copy on Windows, open Command Prompt in the folder with the file and run:

    certutil -hashfile CIBEX_v1.0.html SHA256
