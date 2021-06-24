---
title: Writing Code That Matters
---

[![Image from Gyazo](https://i.gyazo.com/35eff39b0ca2c7bdccd1a3205f77569b.png)](https://gyazo.com/35eff39b0ca2c7bdccd1a3205f77569b)

### Preface

My last month of Lambda School was spent gaining real world experience on a cross-functional team of front and backend developers, data scientists and product managers. Our objective was to create a website for the local non-profit [Family Promise](https://www.familypromiseofspokane.org/). The executive director and case managers needed a way to track and visualize the services they provided. These actionable insights will help the organization apply for more grants and funding.

[![Image from Gyazo](https://i.gyazo.com/66de14594855b662437a7ed7e320a3ce.png)](https://gyazo.com/66de14594855b662437a7ed7e320a3ce)

Family Promise helps local communities coordinate their compassion to address the root causes of family homelessness. They tap existing local resources to empower families towards economic stability. Families come to them in crisis; they help them rebuild their lives with new skills and ongoing support. They address the issue holistically, providing prevention services before families reach crisis, shelter and case management when they come homeless, and stabilization programs once they have secured housing to ensure they remain independent.


Initially, I had some concerns over how sensitive user data was going to be handled. Cloud security is important for the protection of hosted information. A certain amount of confidence is needed when relying on a third-party vendor. Even small gaps in security coverage can put everything at risk. To mitigate these inherent risks, we chose a database service called [Elephant SQL](https://www.elephantsql.com/). The company uses short-lived signed SSH keys and two-factor authentication on every cloud platform (such as AWS and Heroku).

### If You Build It They Will Come

The process of developing the website started with a product roadmap to bridge the gap between what the stakeholder wanted and what the user needed. A stakeholder is anyone who has a stake in what’s being developed. My first thought to determine functionality was to discover the user’s motivation and what they want to achieve on the platform. For example, an employee’s motivation would be to better perform at their job.

I paired up with three data scientists to create this functionality into the following user story.

“As a user, I can see the density of services in a specific area”

The process of breaking down this user story started with the back-end developers. We needed a database to track all the services provided on a daily basis. Next, the data scientists used a SQL query to create the feature. Then, the front-end developers implemented the visualization for the user interface. The main user of this product was going to be out in the field on a tablet. We needed to show the information they wanted in a concise and clear manner.

<iframe width="900" height="500" frameborder="0" scrolling="no" src="//plotly.com/~egrinalds/64.embed"></iframe>

Our team used a service called Whimsical to design the architecture for our cross-functional build. This laid the framework for the front and back-end developers and data scientists. One technical challenge we faced was deploying our Fast API endpoints on AWS to the backend Node server. The data had to be returned as a JSON object. If even one developer on the team didn’t update the dependencies then we couldn’t ship the product. We overcame this challenge by working closely with our technical lead. 

[![Image from Gyazo](https://i.gyazo.com/045b302c089e3ae0a02ac8282791d211.png)](https://gyazo.com/045b302c089e3ae0a02ac8282791d211)


[Github Repository](https://github.com/Lambda-School-Labs/human-rights-first-asylum-ds-a)
