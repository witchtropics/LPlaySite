---
layout: post
title:  "Roots to Branches: A Librarian's Progress"
date:   2021-04-23 17:00
categories: 
---
 ![orange](https://github.com/witchtropics/LPlaySite/blob/3567b6bc1267a91948c70032f3f344e8a597b90d/victoria-bilsborough-hEicHG6GqXQ-unsplash_orange.jpg){:height="500px" width="300px"}

## Initial Goals and Stated Expectations
*What is FSHS? Why did I choose this corpus? What did I hope to learn about the Society?*

The Florida State Horticultural Society (FSHS) is a state-level horticultural society founded in 1888. Its membership includes farmers, scientists, and organizations from around Florida, the United States, and the world. The organization has published the proceedings from its annual meetings since 1888, although from 1888 to 1891 the results were published in the "Florida Farmer and Fruit Grower" (1888) and "The Florida Dispatch Farmer and Fruit Grower" (1889-1891) (Cresap, 1958). 

I chose to pursue studying the FSHS Annual Meeting Proceedings with two goals in mind:

1. To better understand the history of horticultural interests in the state of Florida at the turn of the twentieth century.
2. To develop and practice my skills in cleaning and visualizing data through the lens of computational methods with a topic I was familiar with. 


## Methods of Inquiry and Exploration
*How did I develop a corpus and mine it for data? What data did I find?*

The decision to work with the FSHS Annual Meeting Proceedings arose out of my desire to work with texts that were consistently organized, linked together topically, and (for ease of cleaning) in twentieth century English. My own background as a native Floridian and plant lover directed my interest towards this group, as well as the bounty of records available online. 

Fascimiles (in the form of PDF scans) and OCR plain text files were sourced from HathiTrust and Archive.org. The quality of the OCR plain text files was generally quite high but tables and graphs suffered terribly in the process and were not usable. 

# Cleaning 
*Use of RegEx and R to clean coprus and explore/visualize data (talk about Healy here).*

Regular expressions were used as the primary mode of cleaning the corpus's plain text files. Cleaning focused generally upon removing page headers and page numbers and collapsing extra spaces in the next. The proceedings were also separated into separate sections for easier analysis.

1. Front Matter (these sections contained the Table of Contents, Member Lists, Opening Addresses).
2. Papers and Presentations (these sections contained presentations and submitted reports by Committees and guest speakers, as well as discussions held by members and guests of the Society).
3. Back Matter (these sections contained topical indexes and were not isolated from all proceedings in the corpus)


*Note inconsistencies in spelling either due to human error/variability (in regards to the person typing up the records) and OCR scanning issues*
*Visualization here.*

## Development and Evolution of Research

*Proceedings topics and presentations (first set of data)*

*What did I hope to achieve with finding/clarifying this data? Include visualization.*

My initial research question for this corpus was "How do the interests of the Florida State Horticultural Society change over time? Can these changing interests be tracked by distant reading of the papers and presentations presented during the Society's Annual Meetings?" 

The cleaned Papers and Presentations (PaPr) segments were used for a variety of analytic purposes. Topic modeling using these sections provided some insight into the most common interests of the Society (at least in terms of word frequency).

*Membership metadata (second set of data)*

*Why did I want to gain this additional set of data? What does this add to my research? Include visualization.*



*Do the proceedings and membership data intersect in a meaningful way? (Maybe link via Tableau and see what happens?)*

*What did I learn in this process? What was "made clear"?*

## Sharing and Interacting with the Data

*Development of repository and website, explanation of choices.*


*Creation of Wikidata page for FSHS.*

## Branching Out

*What is the future for this project?*

# Data Potenial 

*How could this data be expanded and used in the future? Who might want to use it? How might I share this research?*

The presentation topic and membership data collected in the last few months presents an entry point for other scholars and myself to begin exploring the past interests of the Florida State Horticultural Society. These corpi present researchers with an opportunity to explore the concerns of Florida-invested horticulturalists, farmers, and scientists, but also the demographics of the individuals participating in the creation and presentation of proceedings materials. Researchers could also explore the current corpus of 1894-1922 texts to evaluate how Florida's horticultural development was affected by World War I.

However, the corpi are far from complete. The FSHS remains an active organization, faithfully publishing its annual meeting proceedings every year (up to 2018, as mentioned on the Society's website). Interested researchers could continue expanding on the list of presentations and their topics for further investigation into how the Society moved through the Depression, World War II, and up to the present day. Similarly, the membership lists could be expanded to the present day, with attention to what committees and topics listed members may be involved with from year to year. 

Potenial researchers may seek to gain a networked view of the Society through the linking of the individuals found on member lists, Society committee membership, and organizations and/or businesses involved in the Society, much in the same way as Ahnert et al. describe Lombardi's ‘BCCI-ICIC & FAB, 1972–91 (4th version)’ in "The Network Turn" (2020). Understanding the way individual, Society, and business interests overlap and influence one another over time seems like an intriguing and ambitious undertaking, but I'm certain the results would be fruitful. 

## Conclusion

## Links

(Github Repository)[]
(Florida State Horticultural Society: Wikidata)[]


# Bibliography

Ahnert, R., Ahnert, S. E., Coleman, C. N., & Weingart, S. B. (2020). The Network Turn: Changing Perspectives in the Humanities. Elements in Publishing and Book Culture. https://doi.org/10.1017/9781108866804

Cresap, I. (Ed.). (1958). Proceedings of the Florida State Horticultural Society, 1888. In Proceedings of the Florida State Horticultural Society (Volumes 1-4, 1888-1891) (Vol. 1). Florida State Horticultural Society. https://journals.flvc.org/fshs/article/view/104306/100229
