# Team Ratula

## Members

Maluki Muthusi Maluki [malukimuthusi@gmail.com](malukimuthusi@gmail.com)

FrankLine Bosire [frankbosire2017@gmail.com](frankbosire2017@gmail.com)

Some Important Links

- Our app is at [https://equity.riviatechs.com](https://equity.riviatechs.com)
- Our API server is at [https://server.equity.riviatechs.com](https://server.equity.riviatechs.com)

## Solution Statement

### Problem Statement II, Configurable MT940 Statements

We decided to handle challenge II, after reviewing all of the provided challenges. We believe this is a challenge that needs a solution that will help customers in the market.

We phrased the problem and came up with a design that addresses the main objectives.

### Objectives

- Develop a configurable widget to download MT940s in various formats e.g xls, pdf, or free formats that allows section and formatting of columns(column layout, content, etc)

- A widget which we would then consume from within equity platform via API calls.

- Provide a daily overview of all movements in a company's account(s)

- Allows business to know their financial position for timely descisions, which supports effective liquidity management. Therefore, this is important in supporting cash forecasting

- Users to be able to select the columns and layout from the raw format via a simple UI

- Easily download the selected MT940 data and corresponding columns in various file types

### Justification of Solution

Through our solution equity bank users will be able to get statements of their transactions in the various way they want.

They can select what they want to be included in the statements reports and also be capable of filtering the statements to what their want.

It is the easy to keep track of their financial transactions.

By offering users to select what they want, it helps to keep the customers happy, and keep using the banks online services.

### Description of the solution

At the very high level, we have build an API that offers flexibility in what you want.

For example, you want to view all the transaction that happened between 01/01/2019 to 02/02/2020 and for those transactions, you only want those that were of type credit to your account. You also want to get only the date and Amount and dowload that data in excel format or a pdf report.

Our query system supports those kind of use cases and other complicated ones.

We have been able to achieve these through the use of data graph solution. We have build our API schema using [graphql](https://graphql.org), an open source query language.

### Benefits

- Improve on customer experience with the product.
- This solution can be used with Equity's various products, like mobiles apps, web apps and even USSD.

### Assumptions

We assume users already have equity bank accounts.

### Conclusion

## Technical Documentation

We have built our solution using open source standards and tools that can be interchanged. The core of our architecture is the graphql query language. Graphql is an open source solution that uses REST APIs.

We have used docker containers so that our code can be deployed on any cloud provider whether on premise or on public.

We have used postgres for storage of data.

We are using a loosely coupled architecture and each layer can be scaled independently to meet the number of requests.

![Architecture](arch.png)

## Solution Access

Link to our app [https://equity.riviatechs.com](https://equity.riviatechs.com)
