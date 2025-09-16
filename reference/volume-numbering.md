# Volume Numbering

## Standards

Holdings statements and item enum/chron/description should conform to the [WRLC Recommendations for Print Periodicals in the Washington Research Library Consortium](https://alma.wrlc.org/books/resources-metadata/page/recommendations-for-print-periodicals-in-the-washington-research-library-consortium) and [WRLC Item Record Description Policies and Templates](https://alma.wrlc.org/books/resources-metadata/page/item-record-description-policies-and-templates#bkmrk-templates-configured).

All holdings statements should conform to Section 5.5 of the [ANSI/NISO Z39.71-2006 (R2011) Holdings Statements for Bibliographic Items](https://groups.niso.org/higherlogic/ws/public/download/18121/Z39.71-2006_\(R2011\).pdf) standard, which is available for consultation where more detail is needed than is provided in the examples below.

## Holding Records

* All regular holdings should be in a single 866 compressed summary holdings statement
* Supplementary issues can be included in an 867 compressed holdings statement
* Index issues can be included in an 868 compressed holdings statement
* Indicate continuous coverage ranges with a hyphen
* Indicate breaks in coverage with a comma

### Examples

{% code title="Numbering restarts annually" %}
```
866 4 1 $$a 2020:no.1-2023:no.4
```
{% endcode %}

{% code title="Ranges with a break" %}
```
866 4 1 $$a v.10:no.1(1910:Jan.)-v.10:no.9(1910:Sep.),v.14:no.2(1914:Feb.)-
v.23:no.12(1923:Dec.)
```
{% endcode %}

{% code title="Ranges with a break" %}
```
866 4 1 $$a v.1(1970)-v.10(1979),v.12:no.3(1981:July)-v.20:no.4(1989:Oct.)
```
{% endcode %}

## Item Records

* We do not create item records for individual serials issues, only for bound volumes (and annuals in the GRC)
* Use the designated fields for enumeration and chronology information:
  * Enumeration A: volume
  * Enumeration B: number
  * Enumeration C: issue
  * Enumeration D: special cases that don't fit in the designated fields
  * Chronology I: year
  * Chronology J: month or season
  * Chronology K: day
* Click "Generate" to create an item description based on the data in the Enum/Chron fields
  * Make sure the description is accurate and manually make any changes if needed

### Examples

<figure><img src="../.gitbook/assets/image (15).png" alt=""><figcaption><p>Bound volume that includes volumes 11-14, from 1984-1988</p></figcaption></figure>

<figure><img src="../.gitbook/assets/image (16).png" alt=""><figcaption><p>Bound volume that contains the July-December issues (numbered 7-12) from 2020 (volume 2)</p></figcaption></figure>

## General Guidelines

* Abbreviate enumeration and chronology
  * Volumes = v.
  * Numbers = no.
  * Issues = iss.
  * Months and seasons: use the full name if 4 letters or less (May, Fall), or abbreviate to 4 characters including the period if longer (Jan., Sum.)
* There should not be any spaces in item description fields or summary holding statements (except for between a spelled out month and day e.g. "2022:May 4")
* Numbering is always notes with the highest level first (2020:May, not May:2020)
* When both enumeration and chronology exist record both, with enumeration first followed by chronology in parentheses

## Additional Examples

* **Single volume, year:**\
  v.1(1997)\
  v.1(1997)-v.2(1998)
* **Volume, number, year:**\
  v.27:no.1(2003)\
  v.27:no.1(2003)-no.2(2003)
* **Volume, number, year, month:** \
  v.17:no.1(2003:Jan.)\
  v.17:no.1(2003:Jan.)-v.17:no.2(2003:Feb.)
* **Volume, number, year, season:** \
  v.15:no.1(1991:Spr.)\
  v.15:no.1(1992:Spr.)-v.15:no.2(1992:Sum.)
* **Volume, number, year, month, day:** \
  v.55:no.31(2003:Oct.03)\
  v.55:no.31(2003:Oct.03)-v.55:no.32(2003:Nov.03)
* **Number, year:** \
  no.5(1998)\
  no.5(1998)-no.52(1999)
* **Year, number (numbering restarts each year):** \
  2022:no.1-4
* **Number, year, month:** \
  no.36(2003:Sep.)\
  no.36(2003:Sep.)-no.37(2003:Oct.)
* **Number, year, month, date:** \
  no.1(1995:Jan.2)\
  no.2(1995:Feb.2)-no.51(1995:June 18)
* **Year, season:** \
  2003:Sum.\
  2003:Sum.-2003:Fall
* **Year, month:** \
  2000:Oct.\
  2000:Oct.-2000:May
* **Year, month, day:**\
  1994:Apr.7\
  1999:Apr.7-1999:Aug.20
