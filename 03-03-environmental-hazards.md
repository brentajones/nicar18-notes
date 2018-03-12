# Uncovering environmental hazards faced by urban children

* Chris Zubak-Skees
* Molly Peterson
* Dylan Purcell

##### Summary

Decaying, pollution-choked schools, old homes with lead paint, toxic soil left behind by shuttered factories and even urban heat islands — all environmental dangers faced by children. This panel will show how to uncover these lurking dangers in your own communities by analyzing often-overlooked data sources and, when data is lacking, doing your own testing. 

## Notes

### Schools near roads

Chris Zubak-Skees

"Can we find all the places where schools are next to busy roads?"

Ultrafine particles spike near highways.

Wanted to nationalize the story and bring it out of academia.

FHA Office of Highway Policy Administration. NCES school dataset.

NCES school data takes addresses, geocodes them, manually correct some of the results, and that's all. Wrong about 16 percent of the time.

Theshold of 500 means being off by a few hundred feet makes your analysis bad.

Things they tried:

Loading all the parcel shapefiles in the country and matching them to school locations. How do you figure out which parcel is the school?

Retrieving Google's database of school points of interest and matching them to NCES data. Both of those are messy.

Neural networks to identify things that look like schools. Terrapattern. A lot of schools don't look like schools anymore, e.g. charter schools.

Ran addresses through Google geocoder instead.

### Urban heat & children's health risk

Molly Peterson

Wanted to know how the people most vulnerable to heat were affected by it.

"I see change", crowdsourced climate data.

Project design/sensor design. Arduino.

Cost around $60 each.

Indoor sensors got temp and humidity every 5 minutes, compared with outside data from nearby airport.

Also published and mapped ER visits for heat-related visits.

Existing data don't capture and existing policies don't address what people are actually going through.

Community engagement project: "Where are the hottest and coolest places?" Collected text message data.

Failures: There's no single prescribed outcome.

Scientists offered lots of feedback.

Renters can use this data in rental disputes.

### Toxic City

[Tipsheet](https://www.dropbox.com/s/q5um23esr707coz/Dylan%20Purcell%20tipsheet.pdf?dl=0)

Dylan Purcell

Lead paint 

Lead paint in rental homes. Only about 500 of 2,700 kids were helped by city health departments.

Most they could get was ZIP code breakdown. Philadelphia started "lead court" where they'd bring landlords in. Slap on the wrist, but a roadmap to addresses.

Tainted soil

No database of toxic soil exists, so they dug up dirt and made one. 500 samples from 114 locations. 3/4 of properties had hazardous lead.

Found locations of former smelters.

Old news clips helped.

Boom in housing stirred up dirt.

Construction workers weren't taking basic steps like watering down dirt.

Used satellite imagery to look at it over time.

After story, the state tested.

Children at risk in school

Mostly lead paint and asbestos. Some mold and pests. Drinking water concerns. Work orders often get delayed.

### Questions

Lead risk score? Do other cities have Lead Court?

How do you determine threshold for emissions?

##### Speakers

Chris Zubak-Skees leads a small team of computational journalists as data editor at the Center for Public Integrity. He was previously the Center's developer, doing analysis and interactive journalism with code. He has been part of teams that have won Meyer, Loeb, Goldsmith and Malofiej awards.

Molly Peterson ([@Mollydacious](https://twitter.com/Mollydacious)) reports on climate and environment for public media and print, including High Country News, NPR, CodeSwitch, KQED, & PRI’s The World. In 2009, while at Southern California Public Radio, she was an IRE finalist in radio for a project investigating faulty pumps in New Orleans. Her latest project documented extreme heat in LA’s San Fernando Valley. She has worked for ISeeChange, a citizen climate observation platform funded in part by NASA.

Dylan Purcell is a data reporter on the Inquirer’s investigative team. He has uncovered low conviction rates for violent crimes, widespread cheating on state tests, and the high rate of newborn deaths after heart surgery at a for-profit hospital. He was a member of the reporting team that won a Pulitzer and IRE award for examining violence in Philadelphia’s public schools. Recently, he’s focused on the dangers of lead exposure faced by urban children. [@dylancpurcell](https://twitter.com/dylancpurcell)

_Description and speakers from [official schedule](https://www.ire.org/events-and-training/event/3189/3693/)_