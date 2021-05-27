---
title: Lambda Labs Cross-Functional Build
subtitle: Human Rights First
---


### Planning

Human Rights First is an international human rights organization that advocates for asylum seekers. The nonpartisan effort believes that holding the US judiciary system accountable is crucial. Current resources available to asylum seeker advocates are outdated, conflicting or missing data. 
Our cross-functional team created an automated tool that allows immigration attorneys to contribute data on judicial asylum decisions. This platform will help lawyers identify patterns and predict future outcomes to better serve their clients.


### Execution

There were no easily accessible datasets for my topic, so I had to get creative. To create custom data, I used a Python’s [Beautiful Soup](https://www.youtube.com/watch?v=ng2o98k983k&t=2467s) web scraping tutorial. Parsing the data from [cars.com](https://www.cars.com/for-sale/searchresults.action/?mdId=21655&mkId=28263&page=1&perPage=100&searchSource=PAGINATION&sort=relevance&stkTypId=28881&zc=99019) was easy because of their user-friendly API. The values came out relatively clean because the script removed symbols and converted strings to integers. Finally, I one-hot encoded the categorical features to numerical so I can fit a model.  

[![Image from Gyazo](https://i.gyazo.com/9140848931b1b7d3e536670496aa638d.png)](https://gyazo.com/9140848931b1b7d3e536670496aa638d)

### Reflection

The delivery process of my feature was easy to implement because I worked with such a great team. One concern we addressed with the stakeholders was the nature of open-source software. The platform could become vulnerable to being used by partisan organizations to advocate for the removal of opposite party-appointed judges. Use by third parties is not something that could be controlled.


[Github Repository](https://github.com/Lambda-School-Labs/human-rights-first-asylum-ds-a)
