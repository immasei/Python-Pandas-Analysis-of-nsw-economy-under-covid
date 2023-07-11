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

- data is general: Data is not divided by state but includes the whole of Australia. However, we assume that it’s the same trend in NSW.

**4. Passenger air movement**

- estimation: Figures may include estimates and figures for some airports for some years may not be complete.

- data isn't a true representation of every airport in NSW: in these 20 airports, there's only 1 airport in NSW.

- type of passenger: It doesn’t include the nationality of passengers. In order to show how travel restrictions impact tourism, airports and economy, we need to know whether people entering Australia from overseas are returning citizens or others.

### Data cleaning & visualising
(Run the Jupyter Notebook)
All cleaned datasets are limited to NSW, from Jan 2019 to Dec 2021. Each dataset contains 37 rows (including header) with strictly 12 months per year. 

### Data Analysis: Covid19 impact on NSW economy
We focus on 3 stages:
2019: pre-covid (prep)
2020: covid (peak)
2021: post-covid (restoration)

**1. International students** have a significant economic impact on Australia. According to Lauries Pearcey, Pro Vice-Chancellor International at UNSW Sydney, for every 3 overseas students studying in Australia, $1 million of economic activity is generated. This includes tuition fees, rent, bills, etc.…

When Australia decides to close their border in Mar 2020 for COVID, many students decide to return to their countries. From Mar 2020 to Dec 2021, Australia remains closed. During the pandemic, many families became financially unstable. Therefore, the number of overseas students in Australia continues to drop (including NSW).

Of all educational sectors, Higher Education (Fig 1.1) has the highest fee (30k ~ 50k~), which means students in this sector are likely to contribute the most to the NSW economy. As we can see, the number of commencements has been gradually decreasing from 2019 (pre-covid) to 2021. The trends predict that if NSW won’t open, then their students will continue to decrease, and directly hit the NSW GDP that gained from exporting education.

For a more general view, (Fig 1.2) highlights the range of number of commencements/ enrolments in every sector. We can see that in 2019, the maximum is 160k students. However, it’s 140k in 2021. If we multiply this range with its frequencies, NSW is losing up to a million students in just 2 years. However, please note that the data also includes students taking online courses, so tuition fee is paid but not accommodation fee.

**2.** According to ABS records, the **transport sector** has a huge role and influence on the country's GDP, with profits generated by transport alone accounting for 4.6% of the country's total GDP in 2015-16, and a further 2.7% increase in the contribution of other areas during this period. During the COVID-19 outbreak in Australia in 2020, many people refused to use public transport in order not to get infected. (Fig 2.1) shows average trips of each year. We can see a significant drop from year 2019 to year 2020. In year 2021, while the ICR is improving, the avarage stays below 2020.

**3. Employment rate** is also an important economic indicator. This indicator represents the proportion of the working age population between 20 and 64 that is currently in employment. It reflects the interplay between number of factors, such as the impact of economic policies on employment levels; the extent to which policies are in place to assist some groups gain entry to employment (e.g., family friendly policies for people with young children); and cultural factors, amongst many others. As a result, the employment rate provides important contextual data about the operation of labor markets across the country, and the way they are affected by different conditions and events.

The unemployment rate is the percentage of people in the labor force who are unemployed. When the unemployment rate is high, it indicates that the country's economic situation is not optimistic. From the (Fig 3.1), we can see that the unemployment rate in Australia is quite stable in 2019, it then began to rise rapidly with the start of the COVID-19 in 2020. This illustrates the severe economic impact of the pandemic in Australia. However. please note that although we assume the same trends in NSW, this data includes the whole Australia.

**4. In terms of **travelling**, as claimed by Tourism Australia, Australia generated $60.8 billion in direct tourism GDP in the financial year 2018-2019. Furthermore, the Australia touristry was its fourth largest exporting industry, accounting for 8.2 percent of its exports income.

Using 2019 (pre-covid) as a normal standard, we could see that airline passenger declined significantly in the following years as the consequences ofborder closures, both international and domestic. From (Fig 4.1), International passenger numbers fell sharply from ~8.5 million inbound and outbound passengers in 2019 to 2 million in 2021 and continued
to decline to ~320k in 2021. (Fig 3.1) The trend means the number of international passengers may continue to decrease if the COVID-19 pandemic continues to outburst. Domestic passenger numbers also fell drastically from ~13.7 million inbound and outbound passengers in 2019 to nearly 4 million in 2020. The decline has been stabilized in 2021 but does not seem to be returning to its peak. 

However, please note that the data only includes 1 airport in NSW, which is Sydney airport. Secondly, the purpose of passengers coming into Australia by air may be other than travel (citizen returning, business, transit.). Therefore, the data may not show the whole picture of NSW touristy status.

**Overall**, border closers, shutdowns, can cause a tremendous affect in GDP. Therefore, we should avoid lockdown at all costs, in which simply following government guidelines of wearing masks, maintaining distances.





