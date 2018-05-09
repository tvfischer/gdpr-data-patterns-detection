# Repository for Detecting Personal Data Patterns in support of GDPR
This Repository has been created to help organisations better understand how to detect data/information that might be affected under GDPR. While large organisations may have the man power and means to secure patterns to detect personal data, this may not be the situation for smaller organisations.
The purpose of this repository is to fill that gap and provide tools to help facilitate the detection of personal information.

## What is GDPR
The General Data Protection Regulation (GDPR) [ (EU) 2016/679 ] is the short form for the EU legislation whose full title is Regulation on the protection of natural persons with regard to the processing of personal data and on the free movement of such data, and repealing Directive 95/46/EC. The regulation was issued on 27th April 2016 and will come into effect, i.e. implemented, on 25th May 2018

GDPR is a regulation issued by the European Parliament​, the European Council​ and European Commission whose purpose is to enhance and unify the processing and protection of an personal data for citizens with-in the European Union (EU). It includes coverage for export of EU personal data to countries outside the union.

[More information](docs/gdprinfomration.md) on GDPR.

### Personal Data Definition
GDPR does define what personal data is with-in Article 4 and thru Recitals 15,26,28,29,30,31,34,35,36,37. To be precise the definition is:
> ‘***personal data***’ means **any information** relating to an identified or identifiable natural person (‘*data subject*’); an identifiable natural person is one who can be identified, directly or indirectly, in particular by reference to an identifier such as a name, an identification number, location data, an online identifier or to one or more factors specific to the physical, physiological, genetic, mental, economic, cultural or social identity of that natural person

## How to Use this Repository
The repository is built around each member state (yes including the UK which will technically still be in the EU at the start of GDPR). Also included is a general set of patterns which will apply to each member nation (e.g. IP addresses, IMEI, DoB, ...)

In each folder, you will find a general country readme describing the invidivual country specific patterns.

## Format of a Pattern Document
Each folder will contain a top level pattern description in [markdown](https://daringfireball.net/projects/markdown/). The file should be in the following format
```
Intro paragraph
Data definitions
* Pattern Name
** Pattern definition and explanation
** Basic regex
** Link to more complex regex
* Next name
Links
List of associated links
```
Following is a brief description of the individual sections:
Intro paragraph - this will be an introduction to explain the key member state personal data identifiers that will be made avaialable in this document.
Data Defintions - this section will be the actaul list of all the different patterns for the member state (or common) personal data elements. This section will have multiple data patterns listed in the following format.
1. Pattern name : the name of the pattern (e.g. UK VAT Number)
2. Pattern defintion : this will describe the pattern as it might be listed in a government website or how it is built.
3. Basic RegEx : this is a general regular expression to match the pattern described in the previous step.
4. Links to more complex RegEx : links to more complex or system specific regular expression (e.g. perl, Autonomy) that can be stored in the subfolder of the member state.

