# How and why to make your data analysis reproducible (a)

**Tipsheet: [bitly.com/reproducible-data](http://www.bitly.com/reproducible-data)**

* [Ryann Grochowski Jones](https://twitter.com/ryanngro)
* [Hannah Recht](https://twitter.com/hannah_recht)
* [Jeremy Singer-Vine](https://twitter.com/JSVine)
* [Hannah Cushman](https://twitter.com/hancush)

##### Description

You understand how you processed your data. Does your editor? Your reader? You, in six months? Without a replicable approach to extracting, transforming and loading data, we are often frustrated in our efforts to share or update our work. Join us for a panel discussion of reproducible data workflows. We’ll talk about why we use standardized processes for collecting, cleaning and analyzing data, and share practices that work for us. We’ll also discuss strategies for smart human intervention (i.e. reporting, logging and documentation) in automated workflows.

## Notes

### What is Data Reproducibility?

**Hannah Recht (HR):** "Whatever you're doing, someone else could reproduce it" whether that's getting the data, analysis, visualization or the story. If you're coding, you run your code and get the same thing every time. Good if you decide to change course halfway through or revisit your data later on.

**Hannah Cushman (HC):** Doesn't necessarily mean fully automated. Even if one part is reproducible, it still makes it easier.

**Jeremy Singer-Vine (JSV):** Inputs and outputs. Inputs should yield the same outputs. "What could I delete from my computer, hit one button and have it regenerate completely?" Reproducibility vs. transparency.

### What is an ETL Process?

**HC:** Extract-transform-load. Extract = get the raw data. Transform = Doing stuff. Load = Publish or load data into news app.

Principles:

* Source data is lava. We don't touch it.
* Process is deterministic: You'll always get the same thing.
* Standard tool kit, standard process. We're all speaking the same language.
* Version control
* Kind code. Kind code is easier to read and understand for you and others.

**JSV:** Series of assumptions and inputs, series of outputs. Could be lots of things — lots of data types. Be explicit about what the findings are. Uses Make (DataMade does too). Goal: One command that deletes all your outputs and runs all your code to reproduce the outputs.

**HR:** Start thinking about reproducibility. First line of script is "Download file". Documenting decisions and processes. 

### How does ETL process guide data exploration

**HC:** Have an auditable trail of things you did to your data. "Freedom to forget". Helpful if your code gives you "sharable artifacts" to help editors, reporters, etc. even if it's not for publication.

**JSV:** Radiating circle: Do it for myself, future self, collaborators, editors, for the public. Also adds accountability. All the other parts are for practicle reasons, making it public is more about the principle.

### What can't be automated and how do you deal with that?

**HC:** Reporting can't be automated. "There's no computer script in the world that can impart meaning on this subjective subject that someone else made."

**HR:** Building your own datasets. Gathering the data sometimes can't be; once you've gathered it, it can.

**JSV:** Anything manual should be part of the input. If there's a part in the middle you can't automate, think of it as two smaller reproducible projects with a step in the middle.

### Example of when reproducibility was valuable:

**HC:** Gives you street cred. Helps you explain things more intelligently to other folks in the newsroom.

**HR:** Saves a lot of work; Factfinder and punching a button hundreds of times or automating it.

**JSV:** Hurricane Harvey-related industrial emissions. New data coming in all the time, wanted to make sure they had the most updated data. Human judgment: Records to ignore — science reporter identified things that had nothing to do with the hurricane.

### Favorite tasks to replicate:

**HC:** SQL queries.

**HR:** Standardizing county names and joining them to FIPS codes.

**JSV:** Everything. Command to re-run all jupyter notebooks and export the output.

### Hardest task to replicate:

**HC:** Chicago lead analysis. Lots of data in PDFs in different formats.

**HR:** Horrible data formats.

**JSV:** Time. Some things take a very long time to run. Figure skating analysis, one cell could take 4-8 hours.

### Good entry point:

**HC:** Take something you've already written and make it reproducible.

**HR:** Take code that's "sort of reproducible" and make it reproducible. More of a mindset rather than a technical skillset.

**JSV:** Write a methodology. "The art of explaining".

## Questions:

### Reproducing your data when it's meant to be live

**HC:** Build in a checking step. Notifies if something is wrong and doesn't push new data to production.

### Testing?

**HR:** Definitely want to test throughout the process. Create logs.

**Ryann Grochowski Jones (RGJ):** System that gives you alerts when stuff doesn't look the way it should. Airflow ETL system.

### How to use on a team?

**HC:** Lots of documentation. Tutorials.

**JSV:** Have some flexibility so it's fun.

**RGJ:** Trainings. Show reporters why it matters.

### Dealing with uncertainty of when something might be a story

**HR:** Do the basic stuff from the beginning, can add later. Assume that at some point it might go somewhere.


##### Speakers

Ryann Grochowski Jones is the deputy editor for data at ProPublica. Previously, she was a data reporter at ProPublica and at Investigative Newsource in San Diego, California. She received her master’s degree from the University of Missouri School of Journalism, where she was a data librarian for IRE/NICAR. Ryann began her career as a municipal beat reporter for her hometown newspaper in Wilkes-Barre, Pennsylvania. [@ryanngro](https://twitter.com/ryanngro)

Hannah Recht is a data journalist at Bloomberg News. She likes scraping obscure insurance filings and wrote an R package that accesses Census data. She previously worked at the Urban Institute as a researcher and data visualization developer. [@hannah_recht](https://twitter.com/hannah_recht)

Jeremy Singer-Vine is the data editor at BuzzFeed News. He also publishes Data Is Plural, a weekly newsletter of useful/curious datasets. [www.jsvine.com](https://www.jsvine.com/)

Hannah Cushman is a journalist turned hacker for public good. She arrived at DataMade, a civic technology company in Chicago, by way of The Associated Press. She believes in open information, empathy, and Dark Matter coffee. [@hancush](https://twitter.com/hancush)

*Description and speakers from [official schedule](https://www.ire.org/events-and-training/event/3189/3532/)*
