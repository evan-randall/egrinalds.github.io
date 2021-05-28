---
title: Human Rights First
---

### Introduction

My last month of Lambda School was spent gaining real world experience on a cross-functional team of data scientists, web developers, product managers and external stakeholders. Our objective was to create a website for [Human Rights First (HRF)](https://www.humanrightsfirst.org/asylum) to advocate for asylum seekers. The international human rights organization is nonpartisan and believes that holding the US judiciary system accountable is crucial. The platform enables immigration attorneys to contribute data for judicial asylum decisions. Then the data helps identify patterns to predict future outcomes so lawyers can better serve their clients. 

[![Image from Gyazo](https://i.gyazo.com/905f197cff1a96d817f0159164a62651.png)](https://gyazo.com/905f197cff1a96d817f0159164a62651)

### If You Build It They Will Come

First, our cross-functional team collaborated on user stories to determine the functionality of the product. User stories are created to break down into concise tasks for developers. My first thought was to determine what is the user’s motivation and what they want to achieve on the platform. We chose a vertical breakdown opposed to the horizontal method because smaller tasks still result in working software. This way functionality will not be split across technical layers but functional layers. Then, the tasks were assigned on a Trello board. 
 
My contribution was to create a feature identifying what asylum cases had been appealed. Our data science team broke down the following user story into these specific tasks. 
“As a user, I can determine if the asylum case was initial or appellate.”

Design an upload template for file to be scanned as pdf
Convert the pdf into an image
Implement Pytesseract for optical character recognition (OCR)
Use SpaCy’s Natural Language Processing (NLP) library to search for keywords like panel members or judges
Aggregate the data to create visualizations for stakeholder


### Overcoming Obstacles

One technical challenge we faced was managing the dependencies of the requirements.txt file because Docker wouldn’t install. The error was caused when we tried using spaCy’s outdated en-core-web-sm library. After upgrading to version 3.0.0, Docker was able to simplify our workflow by sorting the software into packages called containers. Containers were then isolated and bundled their libraries and dependencies.


### Reflection

My main take away from the Labs experience was that agile product development is a team sport. By the end of the product development cycle, there were 12 web developers and 10 data scientists working together! This taught me the importance of time management so we could meet the stakeholder’s deadline. One concern we addressed was the nature of open-source software. The platform could become vulnerable to being used by partisan organizations to advocate for the removal of opposite party-appointed judges. Use by third parties is not something that could be managed.

[Github Repository](https://github.com/Lambda-School-Labs/human-rights-first-asylum-ds-a)
