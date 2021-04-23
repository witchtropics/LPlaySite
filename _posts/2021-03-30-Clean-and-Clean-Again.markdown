---
layout: post
title:  "Clean and Clean Again (Data + Repository)"
date:   2021-03-30 12:30
categories: enriched data, cleaned data
---

#  OCR Can Only Get You So Far 

Very nearly all the way there, in fact. 

In the course of creating the [FSHS Membership Data (1894-1917)](https://github.com/comp-methods-fsu-2021/Florida-State-Horticultural-Society-Annual-Meeting-Proceedings/tree/main/Membership%20Metadata) dataset, I was fortunate to deal with, very generally, plain text that was generally quite clean to begin with. However, there were a number of typographical and organizational inconsistencies that required cleaning so the data could be meaningfully analyzed and visualized. 

For example:
* Street addresses and postal details (PO boxes, "care of" statements) were not consistently placed after a member's name, so the simple copy-pasting of details into a spreadsheet required rearrangement. 
* Similarly, if a member's city was located in Florida, only the city was named. 
* Dissimilar amounts of location data were provided for (by?) each member across all volumes. Some members would include their county of residence, or a name of their estate or home, while many others did not. Separating and interpreting this information for the process of collecting and tabulating the member data was incredibly time consuming.
* Inconsistent application and placement of titles (Mr., Miss, Mrs., Dr., M.D., D.D.S.) throughout the corpus, creating confusion during tabulation.

Another step of the cleaning process that I did not anticipate was the need to create a "Country" column. It was exciting to learn that the Florida State Horticultural Society had members as distant as Northern Ireland, Denmark, Burma, and the Phillipines. However, deciding how to refer to some places was tricky. Would I use modern nation designations for foreign countries or territories, or would I use the period reference? I ultimately chose to use present-day designations since I was pressed for time, but this choice was an unpleasant one to make and I would go back to edit these places into more precise period designations if I were engaged in this project in a long term capacity.

# Missing a Step, Falling Up

Experimentation is fraught with ineffiencies. In the process of transferring copy-pasting member lists directly into the Google Sheet and editing the lines directly in there, I missed an opportunity for pre-cleaning the data. What I realized I should have done (way too late in the process to step back and do it this way) was to:

1. copy the member list from each year (headed by the appropriate year) and paste it in to a central document.
2. Edit this document with regular expressions to remove/correct grammatical errors and OCR inaccuracies.
3. Delimit these collated documents with commas for tabulation.
4. Copy-paste/upload document into Google Sheets for further editing.
5. Collate and continue corrections with OpenRefine.

I  plan to follow a process similar to this in the future. While hand cleaning did offer me the opportunity to get very, very familiar with my data, I feel that this process could have been made briefer through more appropriate application of computational methods and tools. 

# Link
[FSHS Membership Data (1894-1917)](https://github.com/comp-methods-fsu-2021/Florida-State-Horticultural-Society-Annual-Meeting-Proceedings/tree/main/Membership%20Metadata)

## 04/19/2021 Update (...and Clean Again)

# Repository Tidying

Alongside cleaning data, I also reorganized my [repository](https://github.com/comp-methods-fsu-2021/Florida-State-Horticultural-Society-Annual-Meeting-Proceedings) to reflect the types of documents I created. I sought to title the repository's folders clearly to indicate their contents, as well as including brief README files in most of them to explain their contents. While the repository's main README file does not contain a full list of all changes, I hope to continue updating it with links to my other blog posts for more robust details on my progress. 

