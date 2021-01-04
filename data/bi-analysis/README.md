# Technical Case - BI/Analytics

## Context

Petlove is the largest pet-oriented platform in Latin America. The company's role is to take care of the whole pet experience, including supply chain (by e-commerce [here](https://www.petlove.com.br/)), health care (by [Vet Smart](https://www.vetsmart.com.br/)), enterprise management (ERP by [Vetus](https://vetus.com.br/)), and daily care (by [DogHero](https://www.doghero.com.br/)).  In this diverse scenario, Petlove group created data squads carefully planned to join different skills to increment each initiative performance.

Your challenge is to participate in the **Subscription Team,** a service where the pet owner schedules the delivery of a set of items within a custom period subscription and discounts.

## The problem

The Subscription Team has a goal to reduce subscriber churn. **Churn** is any user who signed the Petlove's subscription service and canceled it after hiring.

When analyzing data from the last few months, despite all the usability improvements on the platform, churn has been increasing. Here is the chart to exemplify:

![Churn Progress Over Time](./materials/churn.png)

In the graph, the bar represents the relative number of users who canceled the subscription in the respective month. The dashed line is the goal of the subscription team in which you are inserted. An example to clarify the calculation: in October/2020 of 1,000 subscribers in the base, 75 of them canceled their subscription.

Your job will be **to present a final result with TWO main points: Learnings and Next Steps**. Remember that the insights need to be clear to everyone, from the director of the area to the technology team that will see your presentation.

## Tools

Here are the tools we use and SUGGEST you to use to continue in this process:

1. **Python/Jupyter Notebooks/SQL** ⇒ when code is required;
2. **PowerPoint/Google Slides** ⇒ to present the results to the external team;
3. **GitHub** ⇒ as a repository to store the codes and some - small - documentation. 

## Materials

The data engineering team provided a **SAMPLE** within a csv with the most useful data for you ([link here](https://github.com/petlove/vagas/blob/master/data/bi-analysis/data-test-analytics.csv)). This material will be enough to bring you the expected insights. For analysis, consider the data definition below:

| Column             | Description                                                           |
|--------------------|-----------------------------------------------------------------------|
| id                 | User ID                                                               |
| created_at         | Creation date of the subscription                                     |
| updated_at         | Date the subscription was last updated                                |
| deleted_at         | Date when the subscription was canceled / deleted                     |
| name_hash          | Username, encrypted                                                   |
| email_hash         | User email, encrypted                                                 |
| address_hash       | User address, encrypted                                               |
| birth_date         | User birthday                                                         |
| status             | Subscription status                                                   |
| version            | Subscription version released                                         |
| city               | User city                                                             |
| state              | User state                                                            |
| neighborhood       | User neighborhood                                                     |
| last_date_purchase | Date of last purchase made by subscription                            |
| average_ticket     | The average value of the user for each order                          |
| items_quantity     | The average number of items that the user usually signs               |
| all_revenue        | Total user-generated revenue in subscription                          |
| all_orders         | Total user-generated orders in subscription                           |
| recency            | How many days have passed since the user's last purchase, in recency. |
<br>

## Final delivery

What you are expected to deliver within the test period:

1. **Codes:** whether in python/notebook or SQL, to understand how graphics and insights were calculated;
2. **Technical documentation:** preferably a simple README in markdown, to explain the code logic in more detail;
3. **Final presentation**: can be in PDF or PPTX format, with all the insights to solve this case.

The **criteria for evaluation** are:

1. **Storytelling/Rhetoric:** how easy is for you to explain the concepts? After the presentation, were the insights explicit and the results of the analysis clear?
2. **Quality of your code:** evaluate the performance and ease of reading/understanding the content. Some references for us are: for (general) code best practices ([here](https://www.amazon.com/Clean-Code-Handbook-Software-Craftsmanship/dp/0132350882)), for python itself ([here](https://google.github.io/styleguide/pyguide.html)), and for the SQL itself ([here](https://about.gitlab.com/handbook/business-ops/data-team/platform/sql-style-guide/));
3. **Documentation:** does the material have clear documentation of the calculations logic? There is a suitable README to explain the analysis or final results? Remember, TECHNICAL documentation turns your code easy to be understood, reproduced, and maintained.
4. **Visualization:**  how clear are the graphics, and how explicit are the axes? How simple are the ideas, and how easy is it to communicate the main insights to the business team? The design evaluation considers only the analytical and functional meaning, but NOT the ARTISTIC sense;
5. **Next Steps:**  are the suggested actions useful? Do they solve the Subscription team business pain? Are the next steps clear for everyone during your presentation?

**IMPORTANT:**  no statistical model of churn forecast will be evaluated. Feel free to produce and deliver other results, BUT YOUR PRIORITY is the analysis and the final material for the business/product team.
