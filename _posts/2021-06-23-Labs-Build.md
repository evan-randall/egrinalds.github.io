---
title: Writing Code That Matters
---

[![Image from Gyazo](https://i.gyazo.com/35eff39b0ca2c7bdccd1a3205f77569b.png)](https://gyazo.com/35eff39b0ca2c7bdccd1a3205f77569b)

### Preface

My last month of Lambda School was spent gaining real world experience on a cross-functional team of front and backend developers, data scientists and a product manager. Our objective was to create a website for the local non-profit [Family Promise](https://www.familypromiseofspokane.org/). The executive director and case managers needed a way to track and visualize the services they provided. These actionable insights helped the organization apply for  future grants and funding.

[![Image from Gyazo](https://i.gyazo.com/66de14594855b662437a7ed7e320a3ce.png)](https://gyazo.com/66de14594855b662437a7ed7e320a3ce)

Family Promise helps local communities coordinate their compassion to address the root causes of family homelessness. They tap existing local resources to empower families towards economic stability. Families come to them in crisis; they help them rebuild their lives with new skills and ongoing support. They address the issue holistically, providing prevention services before families reach crisis, shelter and case management when they come homeless, and stabilization programs once they have secured housing to ensure they remain independent.

Initially, I had some concerns over how sensitive user data was going to be handled. Cloud security is important for the protection of hosted information. A certain amount of confidence is needed when relying on a third-party vendor. Even small gaps in security coverage can put everything at risk. To mitigate these inherent risks, we chose a database service called [Elephant SQL](https://www.elephantsql.com/). The company uses short-lived signed SSH keys and two-factor authentication on every cloud platform (such as AWS and Heroku).

### If You Build It They Will Come

Developing the website started with a product roadmap to bridge the gap between what the stakeholder wanted and what the user needed. A stakeholder is anyone who has a stake in what’s being developed and usually includes the customer. My first thought was to determine functionality and to discover the user’s motivation and what they wanted to achieve on the platform. For example, an employee’s motivation would be to better perform at their job. The main user of this product was going to be out in the field using a tablet device. We needed to show the information they wanted in a concise and clear manner. 

I paired up with three data scientists to create this functionality into the following user story.

“As a user, I can see the density of services in a specific area”

<iframe width="900" height="500" frameborder="0" scrolling="no" src="//plotly.com/~egrinalds/64.embed"></iframe>

The process of breaking down this user story started with the back-end developers. We needed a database to track all the services provided on a daily basis. Next, I facilitated communication to ensure the API endpoints were integrated properly. Then, the front-end developers implemented the visualization for the user interface. Last, I reviewed pull requests to prevent merge conflicts on our Github repository. 

The following architecture laid the framework between the three disciplines. The hardest part was making sure every developer had an equal amount of work. The inherent nature of agile development caused the tasks from breaking down user stories to be uneven. A specific technical challenge our team faced was deploying our API to AWS. We had only used Heroku before so the environment variables were different. We overcame this challenge by working closely with our technical project lead. 

[![Image from Gyazo](https://i.gyazo.com/045b302c089e3ae0a02ac8282791d211.png)](https://gyazo.com/045b302c089e3ae0a02ac8282791d211)

The current Data Science [API](http://family-promises-db.eba-saefv7mf.us-east-1.elasticbeanstalk.com) has four endpoints to extract data for key metrics on the analytics dashboard. This solves the executive director’s problem of needing to know how money is spent. The first endpoint is for the map to view the density of services in a specific area. The remaining three endpoints pertain to demographics for age, gender and veteran status. All return a JSON object to be implemented by the front-end developers. The finished product can be seen in the gif below.

[![Image from Gyazo](https://i.gyazo.com/ca2782218cf7fae25d09b5b495ad23f9.gif)](https://gyazo.com/ca2782218cf7fae25d09b5b495ad23f9)

### Reflection

One future feature that could be displayed on the analytics dashboard is the cost of each service provided. Budgeting will help the non-profit be more efficient so they can help as many people as possible. A piece of feedback that I received was that I need to know when to ask for help. Asking for help was difficult for me because I didn’t want to come off imcompetent. I’ve taken steps to resolve this by using the 20 minute rule before reaching out. By setting aside my pride and ego, I don’t waste my time or anyone else’s.

My main take away from the Labs experience was that agile product development is a team sport. By the end of the month, we had four data scientists and 12 web developers working together! One challenge during the delivery process I discovered was the concept of “scope creep”. This translates to a feature taking longer than expected to complete. The solution was to under promise and over deliver. The time management skills I learned this past month will help further my career goals as a Data Scientist. 

[Github Repository](https://github.com/Lambda-School-Labs/family-promise-service-tracker-ds-a)
