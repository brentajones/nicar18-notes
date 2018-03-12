# Tips for harnessing new IRS nonprofit data

[Slides](http://bit.ly/2C9DuQV) | [Tipsheet](http://bit.ly/NICAR18-IRS)

* Andrea Fuller
* Todd Wallack

##### Description

Did you know the IRS recently started uploading most nonprofits' annual financial filings to the web in electronic format? We'll give you an overview of how to download the filings and extract key fields into a database. We'll also cover some of the tricks and pitfalls in working with the new IRS data.

This session will be most useful if: You are either familiar with basic programming or can track down a programmer later to help.

## Notes

**Todd Wallack (TW):** Lots of info in 990s.

Now they're available electronically. More than 2 million filings.

Not everything is there:

* Orgs that file by paper
* Tiny groups that file 990-N
* Groups that don't file at all (churches, etc.)
* Forms that haven't been processed (takes a few months)
* Forms processed before 2011

Format: XML

There are index files for each year, JSON and CSV. They're slightly different.

Approaches to downloading the data:

**TW:** Download all index files, download XML files from indexes, loop through XML files to grab key info, save data in new CSV files. (on GitHub)

**Andrea Fuller (AF):** Download JSON, parse into SQL table, get URLS and download.

##### Speakers

Andrea Fuller is an investigative reporter for The Wall Street Journal in New York City where she specializes in computer-assisted reporting. She is a North Carolina native and previously worked for Gannett Digital, The Center for Public Integrity, and The Chronicle of Higher Education. [@anfuller](https://twitter.com/anfuller)

Todd Wallack is a data journalist and investigative reporter for the Boston Globe’s Spotlight team. He has won national awards for his work on public records and been a finalist for the Pulitzer Prize.  Prior to joining the Globe in 2007, he worked for the San Francisco Chronicle, Boston Herald, and Dayton Daily News. [@twallack](https://twitter.com/twallack)


_Description and speakers from [official schedule](https://www.ire.org/events-and-training/event/3189/3593/)_