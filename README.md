# Latent structures in Household Transactional Data — A societal study 

# Abstract
> A 150 word description of the project idea, goals, dataset used. What story you would like to tell and why? What's the motivation behind your project?


The consumption of everyday commodity products offers the potential to reveal societal inequalities, as well as to identify social milieus including their habits and behaviors. With transactions from more than 2500 households from different societal status over 2 years we try to identify hidden relationships and patterns. The project work will focus on three main aspects: societal implications & structures, health aspects and marketing strategies.

A healthy lifestyle should be one of our top priorities implying that the quality and choice of the food we eat is really important. Hence, we want to assess if people buy high quality food using nutritional values for common ingredients and if there are differences between different groups of people (low/high income, single/with family).

Knowledge about interdependencies and drivers of customer preferences is a crucial factor for effective customer-based strategies. Personalized offers can improve a more precise targeting and successful marketing, satisfying both the customer himself, as well as the retail industry. Further, smart marketing strategies could also be used to change the consumption behavior of households. For instance, the assumed correlation of households with lower incomes buying lower-quality/unhealthy food could be dispersed by placing well-suited advertisements for healthier food.


# Research questions
> A list of research questions you would like to address during the project. 

## Societal Analysis
* Does the income level imply a potential level of education (i.e. do people with higher incomes buy more books and what influence does the amount of children take on it?)?
* What kind of products are promoted? How many promotions do exist on books/educational products? Does the advertising industry push our society towards “bad habits”?

## Quality of food
* Is eating healthy more expensive? Are there differences in the quality of food between low and high income households?  Do people with higher income spend more money on (higher quality) food?
* Do single-person households eat more or less healthy? Do married couples eat more healthy (vs multi-people non-married households)? (Promoting Individualism vs Traditional Family values)
* Do poor people/married people/people who buy unhealthy food buy
strategically (like every saturday) or impulsively? (Education)

## Marketing strategies
* Do lower income people rely on coupons? If so, are there food choices steered by the available coupons? —> Responsibility of Shops? Education?
* Do coupons actually save money or do they just lead to people buying certain brands which are still more expensive?
* What does the grocery shopping behaviour look like time wise? Do families do weekly shopping tours, opposed to students doing daily tours? 
* **Market Basket Analysis**: reveal association between different items — identify items in transactions that are frequently bought together —> [Association Rules] (https://www.saedsayad.com/association_rules.htm)
* **Customer Segmentation**: identify groups/clusters of customers differing in product interest/market participation/response to marketing — come up with potential recommendations for retail (wrt. product placement, promotional efforts, etc.) 
* Analysis on brands (private or national). Which is more expensive? What do people buy? 

# Dataset
> List the dataset(s) you want to use, and some ideas on how do you expect to get, manage, process and enrich it/them. Show us you've read the docs and some examples, and you've a clear idea on what to expect. Discuss data size and format if relevant.

* [Dunnhumby - The complete journey](https://www.dunnhumby.com/careers/engineering/sourcefiles): provides insights of the household transactions of 2500 households over 2 years (collected by Data Science Company Dunnhumby)
* [Nutritional values for common foods and products](https://www.kaggle.com/trolukovich/nutritional-values-for-common-foods-and-products/metadata): provides nutritional values for nearly 9000 ingredients (Data from USDA National Nutrient Database for Standard Reference). The difficulty might be to harmonize the formats of the ingredients between the two datasets.

## Challenges 
* How to merge datasets with very different identifiers (e.g. “BROCCOLI/CAULIFLOWER,CAULIFLOWER WHOLE” vs “broccoli, raw”)?

## Limitations of the dataset 
* no time/location indications
* different identifiers to same concepts —> how to merge?
* demographic data only on 800 households, income very broadly categorized —> potentially reducing the size of the dataset 

# A list of internal milestones up until project milestone 2
Add here a sketch of your planning for the next project milestone.

* 15/11: exploring the dataset and analyze it 
  * Looking at the structure of the data: is the dataset balanced? 
  * Explore features in more detail
  * Basic statistical analysis: simple correlations, mean, variance etc.
  * How much data do we have after filtering/cleaning?
* 17/11: Reducing the research questions and summary of the conclusions drawn from the initial data analysis
* 18/11: Find a way to merge the Dunnhumby dataset with the nutritional information of ingredients
* 22/11: First design/structure of the data story
* 25/11: Return for second milestone

# Questions for TA’s
> Add here some questions you have for us, in general or project-specific.







