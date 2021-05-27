---
title: Lambda Labs
subtitle: Human Rights First
---


### Planning

Human Rights First is an international human rights organization that advocates for asylum seekers. The nonpartisan effort believes that holding the US judiciary system accountable is crucial. Current resources available to asylum seeker advocates are outdated, conflicting or missing data. 
Our cross-functional team created an automated tool that allows immigration attorneys to contribute data on judicial asylum decisions. This platform will help lawyers identify patterns and predict future outcomes to better serve their clients.

[![Image from Gyazo](https://i.gyazo.com/905f197cff1a96d817f0159164a62651.png)](https://gyazo.com/905f197cff1a96d817f0159164a62651)

### Execution

In order to recognize outcome trends, the data scientists had to identify key variables or features. My contribution was to create a case type field identifying what asylum cases had been appealed. Just over 80% of cases were appealed!  Then, I created a branch off the main github repository and then created a pull request with my changes. Last, I implemented the feature by using a plotly dash visualization and connecting the JSON output to the Fast API endpoints. 

[![Image from Gyazo](https://i.gyazo.com/9140848931b1b7d3e536670496aa638d.png)](https://gyazo.com/9140848931b1b7d3e536670496aa638d)

### Reflection

The delivery process of my feature was easy to implement because I worked with such a great team. One concern we addressed with the stakeholders was the nature of open-source software. The platform could become vulnerable to being used by partisan organizations to advocate for the removal of opposite party-appointed judges. Use by third parties is not something that could be controlled.

[Github Repository](https://github.com/Lambda-School-Labs/human-rights-first-asylum-ds-a)
