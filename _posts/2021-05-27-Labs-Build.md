---
title: Human Rights First
---


### Ideation

Human Rights First is an international human rights organization that advocates for asylum seekers. The nonpartisan effort believes that holding the US judiciary system accountable is crucial. Our cross-functional team included a product manager, web developers and data scientists. We created an automated tool that allows immigration attorneys to contribute data on judicial asylum decisions. This platform will help lawyers identify patterns and predict future outcomes to better serve their clients.

[![Image from Gyazo](https://i.gyazo.com/905f197cff1a96d817f0159164a62651.png)](https://gyazo.com/905f197cff1a96d817f0159164a62651)

### Planning

In order to recognize outcome trends, the data scientists had to identify key features. My contribution was to create a case type field identifying what asylum cases had been appealed. I broke down the following user story into specific tasks.

“As a user, I can determine if the asylum case was initial or appellate.”

1. Design an upload template for file to be scanned as pdf
2. Convert the pdf into an image
3. Implement Pytesseract for optical character recognition (OCR)
4. Use natural language processing (NLP) to search for keywords like panel members or judges
5. Create visualization to quantify the rate of cases getting appealed

### Execution

The user story could be completed in 6 months because of the planning, coding and debugging involved. The product has already been in production for 5 months so a majority of the planning and coding is complete. The existing code base had implemented the template, optical character recognition (OCR) and natural language processing (NLP) functionality. The last month would be spent debugging and collaborating with the stakeholders, web developers and existing user feedback.


### Processes

The complexity of using multiple languages and architectures in the recent Labs project required us to use Docker. This service simplified our workflow by sorting the software into packages called containers. Containers were then isolated and bundled their libraries and dependencies. A technical decision I made was to update the dependencies in the requirements.txt file because Docker wouldn’t install. The error was caused when I tried using spaCy’s outdated en-core-web-sm library. After upgrading to version 3.0.0, Docker was able to run. I advised the decision with my technical lead to ensure the change wouldn’t affect the team.

### Reflection

My main take away from the Labs experience was that agile product development is a team sport. By the end of the product development cycle, there were 12 web developers and 10 data scientists working together! This taught me the importance of time management so we could meet the stakeholder’s deadline. One concern we addressed was the nature of open-source software. The platform could become vulnerable to being used by partisan organizations to advocate for the removal of opposite party-appointed judges. Use by third parties is not something that could be controlled.

[Github Repository](https://github.com/Lambda-School-Labs/human-rights-first-asylum-ds-a)
