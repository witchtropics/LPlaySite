---
layout: post
title:  "Linking and Wikidata"
date:   2021-03-16 23:30:00 -0500
categories: linking
---

## Getting data from Wikidata

Composing a query for my data was relatively straightforward. 

I searched for the term "horticultural" in the Wikidata search bar and selected the auto-suggested result for the [Royal Horticultral Society](https://www.wikidata.org/wiki/Q1032739). The Royal Horticultural Society was listed as an instance of ["horticultural society"](https://www.wikidata.org/wiki/Q5906761). 

I ran a query through the Filter setting for "instance of" "horticultural society" per the Royal Horticultural Society entry.  

The SPARQL query looks like this: 

```
SELECT ?horticultural_society ?horticultural_societyLabel WHERE {
  SERVICE wikibase:label { bd:serviceParam wikibase:language "[AUTO_LANGUAGE],en". }
  ?horticultural_society wdt:P31 wd:Q5906761.
}
LIMIT 100
```
 and produced a short [list](https://w.wiki/36fL) of horticultural societies from around the globe. The Florida State Horticulural Society is notably absent. 
 

## Giving data to Wikidata

This part was the most challenging in that I wasn't entirely sure what Wikidata  records would be best for me to submit to. I scrolled through the "horticultural society" page and found that the Wiktionary entry for "horticultural society" was unfilled. However, there was no definition available on Wiktionary for "horticultural society", but one was available for "horticulture". I decided to add the Wiktionary definition of "horticulture" to the ["horticulture" record](https://www.wikidata.org/wiki/Q48803), since that had not yet been completed.

