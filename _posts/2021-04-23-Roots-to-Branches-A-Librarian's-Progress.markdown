---
layout: post
title:  "Roots to Branches: A Look at the Progress and Future of This Project"
date:   2021-04-23 17:00
categories: 
---

# Initial Goals and Stated Expectations

The Florida State Horticultural Society (FSHS) is a state-level horticultural society founded in 1888. Its membership includes farmers, scientists, and organizations from around Florida, the United States, and the world. The organization has published the proceedings from its annual meetings since 1888, although from 1888 to 1891 the results were published in the "Florida Farmer and Fruit Grower" (1888) and "The Florida Dispatch Farmer and Fruit Grower" (1889-1891) (Cresap, 1958). 

I chose to pursue studying the FSHS Annual Meeting Proceedings with two goals in mind:

1. To better understand the history of horticultural interests in the state of Florida at the turn of the twentieth century.
2. To develop and practice my skills in cleaning and visualizing data through the lens of computational methods with a topic I was familiar with. 

# Methods of Inquiry and Exploration

The decision to work with the FSHS Annual Meeting Proceedings arose out of my desire to work with texts that were consistently organized, linked together topically, and (for ease of cleaning) in twentieth century English. My own background as a native Floridian and plant lover directed my interest towards this group, as well as the bounty of records available online. 

I sourced fascimiles (in the form of PDF scans) and OCR plain text files from HathiTrust and Archive.org. The quality of the OCR plain text files was generally quite high but tables and graphs suffered terribly in the process and were not usable. 

# Cleaning 

Regular expressions were used as the primary mode of cleaning the corpus's plain text files. Cleaning focused generally upon removing page headers and page numbers and collapsing extra lines and spaces. The OCR plain text files contained two kinds of errors and/or inconsistencies that made cleaning difficult:

1. Inconsistent formatting and spelling in the original published iteration of the proceedings. While the overall structure and order of the proceedings remained very similar from year to year, there were noticeable inconsistencies and errors in both how member names and cities were spelled in the original text, as well as how title and address information was ordered for each member. 
2. OCR scanning errors. Mangled tables and misspelled words were the main results of OCR scanning errors. These errors made searching for and locating segments of text (say, "FLORIDA STATE HORTICVLTVAL SOCIETY ") difficult to completely remove. Similarly, misscanned member and city names were not usually visible until the membership data had been compiled into tabular form, creating the need for a second level of cleaning on a more hands-on level, since many errors were unique in their configuration. 

The proceedings were also separated into separate sections for easier analysis.

1. Front Matter/Prefaces and Addresses (these sections contained the Table of Contents, Member Lists, Opening Addresses). I sourced the member lists for each year from these sections of the annual proceedings.
2. Papers and Presentations (these sections contained presentations and submitted reports by Committees and guest speakers, as well as discussions held by members and guests of the Society). I sourced thed
3. Back Matter (these sections contained topical indexes and were not isolated from all proceedings in the corpus)

# Development and Evolution of Research

My initial research question for this corpus was "How do the interests of the Florida State Horticultural Society change over time? Can these changing interests be tracked by distant reading of the papers and presentations presented during the Society's Annual Meetings?" 

The cleaned Papers and Presentations (PaPr) segments were used for a variety of analytic purposes. [Topic modeling](https://witchtropics.github.io/LPlaySite/topic/modeling/2021/03/10/topic-modeling.html) using these sections provided some insight into the most common interests of the Society. However, using only the presentation topic data to examine the Society's interests felt a bit limited. These presentations and reports were created by committees and not to examine the membership lists seemed short-sighted. 

Compiling the membership lists into a cohesive membership list was an exhausting task, especially when the member names were fraught with so many spelling/OCR errors. It was a largely promising effort, however, revealing the global reach of and interest in Florida horticulture. I was able to create a visualization in Tableau based on the location data available in the membership lists. 

<iframe src="https://public.tableau.com/views/MemberMapCities1894-1917/Sheet1?:language=en&:display_count=y&:origin=viz_share_link:showVizHome=no&:embed=true"
 width="750" height="955"></iframe>


# Sharing and Interacting with the Data

The data for this project is made available on my GitHub repository (linked below), where it is continuously updated as I clean, edit, and expand it. The two main data types (presentation topic information and membership metadata) are kept in separate folders so they may be explored and downloaded one at a time. Please explore the README files for further information. 

I have also created an extremely basic Wikidata page (linked below) for the Florida State Horticultural Society as a first step towards bringing the organization into a world of linked open data. It lacks many of the data points that can be found on the pages of other horticultural organizations because that information wasn't readily available on the FSHS's website. However, it may be easily obtainable through a simple email to the organization.

This website exists as a public-facing opportunity for more of a conversation and reflection of the work being done and doesn't contain quite the technical details of the GitHub logs and READMEs. Unfortunately this also means it's less likely to be updated very often. For more nuts and bolts information, refer to the repository updates. 

# Branching Out

The future for this project is unknown. It began and exists as a means of practicing a number of computational methods for my graduate degree, and its path may very well end there. I do implore interested individuals to use this data if they find it relevant to their efforts, and to let me know about it!

# Data Potenial 

The presentation topic and membership data collected in the last few months presents an entry point for other scholars and myself to begin exploring the past interests of the Florida State Horticultural Society. These corpi present researchers with an opportunity to explore the concerns of Florida-invested horticulturalists, farmers, and scientists, but also the demographics of the individuals participating in the creation and presentation of proceedings materials. Researchers could also explore the current corpus of 1894-1922 texts to evaluate how Florida's horticultural development was affected by World War I.

However, the corpi are far from complete. The FSHS remains an active organization, faithfully publishing its annual meeting proceedings every year (up to 2018, as mentioned on the Society's website). Interested researchers could continue expanding on the list of presentations and their topics for further investigation into how the Society moved through the Depression, World War II, and up to the present day. Similarly, the membership lists could be expanded to the present day, with attention to what committees and topics listed members may be involved with from year to year. 

Potenial researchers may seek to gain a networked view of the Society through the linking of the individuals found on member lists, Society committee membership, and organizations and/or businesses involved in the Society, much in the same way as Ahnert et al. describe Lombardi's ‘BCCI-ICIC & FAB, 1972–91 (4th version)’ in "The Network Turn" (2020). Understanding the way individual, Society, and business interests overlap and influence one another over time seems like an intriguing and ambitious undertaking, but I'm certain the results would be fruitful. 

# Links

[GitHub Repository](https://github.com/comp-methods-fsu-2021/Florida-State-Horticultural-Society-Annual-Meeting-Proceedings)

[Florida State Horticultural Society: Wikidata](https://www.wikidata.org/wiki/Q106520514)


# Bibliography

Ahnert, R., Ahnert, S. E., Coleman, C. N., & Weingart, S. B. (2020). The Network Turn: Changing Perspectives in the Humanities. Elements in Publishing and Book Culture. [https://doi.org/10.1017/9781108866804](https://doi.org/10.1017/9781108866804)

Cresap, I. (Ed.). (1958). Proceedings of the Florida State Horticultural Society, 1888. In Proceedings of the Florida State Horticultural Society (Volumes 1-4, 1888-1891) (Vol. 1). Florida State Horticultural Society. [https://journals.flvc.org/fshs/article/view/104306/100229](https://journals.flvc.org/fshs/article/view/104306/100229) 
