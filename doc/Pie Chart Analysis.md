# Pie Chart for Frequency of Income Groups

## Overview
The pie chart provides a visual representation of income group distribution, emphasizing economic diversity and its impact on life expectancy.

## Key Findings
- Highlights the unequal distribution of countries across income groups.
- Underlines the need for targeted interventions in lower-income countries.

## Code Snippet
```sas
proc template;
	define statgraph SASStudio.Pie;
		begingraph;
		layout region;
		piechart category=Income_Group /;
		endlayout;
		endgraph;
	end;
run;

ods graphics / reset width=6.4in height=4.8in imagemap;
proc sgrender template=SASStudio.Pie data=MYDATA.PROJECT2;
run;
ods graphics / reset;
