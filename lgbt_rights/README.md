
# Wikipedia Data on LGBT Rights

<a href="https://en.wikipedia.org/wiki/LGBT_rights_by_country_or_territory">Wikipedia data</a> will be used to rate national laws regarding LGBT rights.

## The Data

For simplicity we will consider the data tables in the article referenced above. More specifically, the categories are:
<ul>
	<li>Same-sex sexual activity</li>	
	<li>Recognition of same-sex unions</li>	
	<li>Same-sex marriage</li>	
	<li>Adoption by same-sex couples</li>	
	<li>LGB allowed to serve openly in military?</li>	
	<li>Anti-discrimination laws concerning sexual orientation</li>	
	<li>Laws concerning gender identity/expression</li>
</ul>

## Scoring 

Each country will be scored on the basis of the aforementioned criteria. Depending on whether there is a tick, cross or both in a column column (criterion) for a country, the score for that criterion will be 1, 0 or 0.5 respectively.

The final score for a country is the average across all criteria.


## Extracting the data

First, we get a list of countries and their iso codes (obtaining_data/1. Get iso data.ipynb).

We then carry out data scrubbing manually to create country_matches.csv -- a 2-column csv file where column one has country names as they appear in the LGBT page and column 2 has country names as they appear in the iso table in wikipedia.

Finally, we use the second python script (obtaining_data/2.... .py) to extract the lgbt data.

## Visualisation

On the website the visualisation is embedded within Nupinion's infrastructure. Here however we provide d3 code for a standalone map viz.