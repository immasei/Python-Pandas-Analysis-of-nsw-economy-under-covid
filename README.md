# How covid impact the economy in Australia, especially in NSW?

## Purpose
COVID-19 officially started from January 2020 and still hasn't ended. It leaves heavy impacts on societies, health and economies. Still, there are people who haven’t been affected by the pandemic and some of them are very subjective. Therefore, we aim to highlight the seriousness of COVID-19 using supporting statistics, to raise awareness of people who travel by public transport, that they should follow the mask guidelines.

In order to find out the economic consequences leaved by COVID-19 in Australia
(NSW), we find 4 data sets, which are about:

1. number of international students in enrolments and commencements

2. transport usage
 
3. (un)employment rate
 
4. number of passengers in and out at 20 airports
   
These data sets are recorded for every month for several years. We expect that in 2020 all data should decrease due to border closure, lockdowns, business difficulties and flight restrictions. Decreases in enrolments, employments, transport usages and flights (travel) will indeed show the impact on the economy.

## Data

### Data origin

| Dataset   | Type | Source  | 
| :-------- | :--: | :------ |
| International Students| excel | [DESE](https://www.education.gov.au/resources/international-education-data-and-research)| 
| OPAL trip counts | excel | [OpenData](https://opendata.transport.nsw.gov.au/user/logindestination=node/10468) | 
| Employment | excel | [ABS](https://www.abs.gov.au/statistics/labour/employment-and-unemployment/labour-force-australia/jul-2022) |
| Passenger Air Movement | excel | [BITRE](https://data.gov.au/dataset/ds-dga-cc5d888f-5850-47f3-815d-08289b22f5a8/details)|

### Data limitation
**1. International Students**

- double count: A student attending two different courses in the same reference period (for example ELICOS and bachelor’s degree) will have both enrolments counted.

- type of students: Overseas students on Australian funded scholarships/ sponsorships or students undertakingstudy while holding tourist or other temporary entry visas (or their dependents) are not recorded. New Zealand students are not included.

**2. Opal Trip Counts**

- empty cells: When separated by mode of transport, it contains a lot of empty cells that need to be handled. There are too few records of Metro in the original dataset, so when I use Travel modes columns to restructure the dataset, too many nan values in the new Metro column.

**3. Employment**

- data is general: - Data is not divided by state but includes the whole of Australia. However, we assume that it’s the same trend in NSW.

**4. Passenger air movement**

- estimation: Figures may include estimates and figures for some airports for some years may not be complete.

- data isn't a true representation of every airport in NSW: in these 20 airports, there's only 1 airport in NSW.

- type of passenger: It doesn’t include the nationality of passengers. In order to show how travel restrictions impact tourism, airports and economy, we need to know whether people entering Australia from overseas are returning citizens or others.

### Data cleaning
(Run the Jupyter Notebook)



