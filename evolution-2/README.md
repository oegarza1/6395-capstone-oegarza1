# Evolution 2: Data Management Competency Assessment

**Oscar Garza | CIDM 6350 and CIDM 6355**

## Current preparedness

My preparation in Data Management connects the design of operational databases with the preparation of data for analysis. CIDM 6350, Data and Information Management, strengthened my understanding of relational modeling, normalization, and integrity constraints. CIDM 6355, Data Mining Methods, extended that foundation by requiring me to transform records into datasets that address specific business questions. Together, these courses helped me see how decisions about structure and meaning influence both software behavior and analytical conclusions.

As a software engineer in financial services, I apply this perspective to an e-commerce payment platform. My experience includes authorization, refund, and verification APIs, as well as customer-profile services. I work with Java APIs hosted in AWS and can implement storage and CRUD operations using DynamoDB or MySQL. Building on my [Evolution 0 assessment](../evolution-0/README.md), I am confident designing schemas and selecting keys and indexes, particularly when considering frequently accessed tables. My next priorities are deeper expertise in database performance and data migrations, along with greater independence in preparing operational data for analysis.

## What I know: database design and supporting evidence

I intentionally based my CIDM 6350 project on my payment-platform experience. The [payment-system relational diagram](https://github.com/oegarza1/6350-data-info-management-assignments/blob/main/Project/CIDM_6350_PROJECT_3RD_FORM_GARZA_OSCAR.drawio) organizes customers, merchants, payment methods, transactions, sales, refunds, and auditing into related structures. For example, payment methods reference customers, transactions reference customers, merchants, and payment methods, and refunds include a reference to the original sale. A customer-onboarding relation connects customers and merchants while recording the onboarding date.

These choices demonstrate my ability to translate a familiar business process into an explicit data model. Separating entities and linking them through keys supports the goal of reducing redundancy while preserving relationships needed by the application. The diagram also includes relations connecting audits with transactions and employees, showing how the model extends beyond payment processing to supporting activities. This artifact demonstrates relational design and normalization work; evidence of implementation and measured performance would be needed to establish how the design behaves under load.

The project reflects a strength I can carry into future settings: understanding how records should relate before implementing the operations that create and modify them. In my professional work, schema, key, and index choices are closely connected to the access patterns an API must support. I am comfortable making those foundational choices, while recognizing that more complex relationships and workloads require additional investigation.

## Preparing data for a business objective

My CIDM 6355 [Uber demand project](https://github.com/oegarza1/6355-data-mining-methods-assignments/blob/master/Garza_Oscar_FinalProject.ipynb) best represents my own direction because I had more discretion in selecting its focus. Using April 2014 New York City pickup data, I converted timestamps, aggregated individual pickups into hourly counts, and derived hour, weekday, weekend, and lag features. I defined high-demand hours using the median pickup count and constructed a preprocessing pipeline with missing-value imputation, scaling, and categorical encoding before logistic regression.

From a Data Management perspective, the central accomplishment is transforming event records into a dataset with a different unit of observation: one row per hour. That change makes the business question manageable, but also determines which distinctions remain visible. Aggregating across locations, for example, removes geographic detail from the modeling table. The project reinforced my need to look beyond the volume of available data and identify what the business objective actually requires.

The [Netflix engagement notebook](https://github.com/oegarza1/6355-data-mining-methods-assignments/blob/master/Netflix_Engagement_Garza_Oscar.ipynb) provides complementary evidence. I documented fields in a data dictionary, standardized session-outcome text, derived viewing-time features, summarized missing values, and separated numeric and categorical predictors. The preprocessing supports comparisons among classification models. Both assignments show that preparation involves decisions about meaning, not simply changing formats. My concern when combining large datasets is ensuring that assumptions, unmatched records, or duplicated relationships do not distort the result. I want to make checks on record counts, key uniqueness, and excluded observations a more consistent part of my workflow.

## Limitations and areas for growth

Complex relationships and slow queries have also challenged me. Although I am confident selecting keys and indexes, diagnosing why a query performs poorly across a larger set of relationships requires more experience. I want to strengthen my ability to interpret execution plans, assess index tradeoffs, and measure the effect of changes under representative workloads. Data migration is another priority: I want to become more capable of planning schema changes, validating transferred records, and preserving application behavior during transitions.

Access controls are an area of confidence. Preparing operational data for analysis is also within my current graduate-level capabilities, although I want to complete that work more effectively with less guidance. Potential gaps I should investigate include how schema changes affect downstream datasets and how missing or excluded records influence conclusions. These questions connect database maintenance to the reliability of the analysis built on it.

## Learning resources and professional judgment

My learning relied primarily on course instruction, assignment materials, and AI assistance. The Netflix notebook contains structured prompts for a data dictionary, preprocessing, and evaluation. The Uber notebook records my use of earlier assignments as templates, with modifications for the selected problem. Both notebooks disclose ChatGPT and Gemini assistance with questions, output review, and ideas. These artifacts document the instructional support behind my work.

AI can help me investigate an error or consider alternative approaches, but I remain responsible for judging whether a suggestion preserves the intended relationships and business meaning. A query that runs faster or a model that reports a higher score still requires careful examination. My development depends on becoming more deliberate about that review and explaining why a technical choice is appropriate.

## Integration and capstone readiness

Data Management connects all four curricular areas by providing a reliable structure for shared information. Data Analytics depends on consistent definitions, appropriate aggregation, and traceable transformations. Software Systems implements the APIs and workflows that create and maintain records. Networking and Cybersecurity supports protected communication and controlled access to those records. In my payment-platform work, these areas meet whenever an API updates a profile, retrieves related information, or generates metadata for performance analysis.

My capstone scope remains undecided, but I am open to adapting the payment-system design if it supports the final project. A manageable prototype could demonstrate a subset of customer-profile or payment relationships using synthetic data, Java APIs, and a documented database schema. It could include analytical queries and a measured comparison of query performance before and after an indexing change. The portfolio would connect design artifacts to implementation evidence, while the presentation would explain the business purpose, design decisions, and limitations.

I am prepared to contribute database design, application integration, and data preparation to that work. My broader capability is to connect how a fintech system stores and maintains information with how that information is protected, analyzed, and used to improve the service. Strengthening performance analysis, migration practices, and dataset validation will make that contribution more independent and defensible.
