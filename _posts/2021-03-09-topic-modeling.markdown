---
layout: post
title:  "Topic Modeling"
date:   2021-03-09 22:52:44 -0500
categories: topic modeling
---

This week's endeavors focused on first attempts at topic modeling. 


## Out of the Spreadsheet and Into the (Text) Files
As a first step, I was to produce a folder of plain text files to be modeled. I wanted to investigate the text of the first 25 (later 40) entries in my collected Florida State Horticultural Society Annual Meeting Proceedings (1894-1922), so I knew I would want to isolate and export the contents of Row I in FSHS_AllProceedings - Sheet 1. This would have been time consuming with the minimum 12 files, so I looked for an R script to help me fast track the task. 

I found some useful results on [Stack Overflow](https://stackoverflow.com/questions/38451768/convert-data-frame-with-one-column-into-txt-documents-one-txt-document-per-row) that I was able to modify to be useful to my work. The code block, unmodified from the linked post, can be found below.

```
for(i in 1:nrow(df)){
  write.table(df[i,],paste0("line",i,".txt"),row.names=FALSE,col.names = FALSE)
}
```
After some tinkering and help through Dr. Hanley's workshop hours, I was able to obtain not-quite-40 (the total came to 22 text of 40 requested) but still a robust collection of text documents to use for my research. 

It is important to note that all files pulled for this exercise are from 1894. 

## Producing a Metadata Table

I produced a metadata table containing each text's 

- Title
- Author
- Year
- Volume
- Word Count

## Taking a Shot at Topic Models

After installing TopicModelingTool and setting up my input and export folders, I decided to see what ten topics the modeling tool may detect.

| Topic ID  | Top Words...  |   |
|---|---|---|
| 0  | trees prof tree scale Ã¢ orange insects leaves solution disease rolfs work sulphur young state destroy red generally pounds blight   | 
| 1  | grapes grape prices good south vines ground car state chicago wright crate market roots vineyard received cents york feet vine  | 
| 2  | Ã¢ mr fruit good years year florida time trees put made make 1 growing place land found orange state ago  |   
| 3 | texas society tropical fruits horticultural state gulf region coast plants committee country states horticulture association meeting introduction varieties great california  |   
| 4  | Ã¢ potash ammonia acid 3 plant lime fertilizer grade cent sulphate cd phosphoric soil soda nitrate form results food salt  |   
| 5  | varieties oranges blood st citron citrus sweet fruits berry strawberry qualities lime cross malta crosses seeds moisture 1 limonia mandarin  |   
| 6  | fly rosin white wash spray webber prof soda scale effective Ã¢ caustic water found gallons eggs insects pest juice cent  |   
| 7  | disease scale florida california horticultural state insect pest moth gypsy fluted olive jose importation vine society imported san source brought  |   
| 8  | manure stable grass fertilizer fertilizers potash seed ground good potatoes phosphate bermuda plant soil man vegetables straw oranges grow grove  |   
| 9  |  fruit trees varieties blight peach pears market box boxes orchard pear limbs chicago barrels tree le harvey persimmon peaches shipped |   

I was surprised at the prominence of grapes and grape growing in Topic 1. Fertilizers (Topic 8) and blight (Topic 9) are reflective of more expected topics to come out of this exercise. 

## Reference Models

I was able to locate reference models on Archive.org in the form of [Missouri State Horticultural Society Annual Proceedings](https://archive.org/search.php?query=creator%3A%22Missouri+State+Horticultural+Society%22). These proceedings are from the same time period (late 19th century to early 20th century) and are formatted and digitized in similar manners. 



