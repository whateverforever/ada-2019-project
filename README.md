# Latent structures in Household Transactional Data — A societal study identifying meat consumption patterns

# Abstract
> A 150 word description of the project idea, goals, dataset used. What story you would like to tell and why? What's the motivation behind your project?

The consumption of everyday commodity products offers the potential to reveal societal inequalities, as well as to identify social milieus including their habits and behaviors. With transactions from more than 2500 households from different societal status over 2 years we try to identify hidden relationships and patterns. This project work will focus on two consecutive interwined aspects: societal latent structures in consumption and transaction behavior and vegetarianism.

This dataset offers the chance to link societal status, income and living constellations to a topic which gains more and more importance in recent times with growing concerns in **climate change: our meat consumption**. This form of _human diet_ can actively promote a change in the amount of greenhouse-gas emissions [[Nature 572, 291-292 (2019)](https://www.nature.com/articles/d41586-019-02409-7)].

Knowledge about interdependencies and drivers of customer preferences and behaviors is a crucial factor for effective customer-based strategies. With this knowlegde at hand, it might be possible to develop new strategies to actively take influence on improving awareness for meat consumption via more precisely targeted advertisements and promotions, satisfying both the customer himself, as well as the retail industry. For instance, the assumed correlation of households with lower income households exhibiting a less balanced/more meat-focused food could be dispersed by placing well-suited advertisements for more vegetarian food.

# Research questions
> A list of research questions you would like to address during the project. 

## Societal Analysis
* **Do the food consumption patterns/habits reflect the belonging to a social class?**
* What kind of products are promoted? 
  * How many promotions do exist on books/educational products? Does the advertising industry push our society towards “bad habits”?
  * Does the income level imply a potential level of education (i.e. do people with higher incomes buy more books and what influence does the amount of children take on it?)? 

## Vegetarianism
* **What is the proportion of vegetarian products in the total houshold spendings? (i.e. how much money is spent on healthy foods?)**
    * Does vegetarianism and the awarneess correlate with the level of income, i.e. social status?
    * Do single-person households consume less meat than families (avg. per person)? 

## Marketing strategies
_Identify clusters._
**Customer Segmentation**: identify groups/clusters of customers differing in product interest/market participation/response to marketing — come up with potential recommendations for retail (wrt. product placement, promotional efforts, etc.) 

_Analysis on clusters and their commonalities & diferences._
* Do lower income people rely on coupons? If so, are there food choices steered by the available coupons? —> Responsibility of Shops? Education?
* Do different households with different levels of income exhibit different buying strategies (i.e. grocery shopping once a week or only buying products on promotion)? 
* Does the use of coupons actually save money or do they just lead to people buying certain brands which are still more expensive?

# Dataset
> List the dataset(s) you want to use, and some ideas on how do you expect to get, manage, process and enrich it/them. Show us you've read the docs and some examples, and you've a clear idea on what to expect. Discuss data size and format if relevant.

* [Dunnhumby - The complete journey](https://www.dunnhumby.com/careers/engineering/sourcefiles): provides insights of the household transactions of 2500 households over 2 years (collected by Data Science Company Dunnhumby)
* [Nutritional values for common foods and products](https://www.kaggle.com/trolukovich/nutritional-values-for-common-foods-and-products/metadata): provides nutritional values for nearly 9000 ingredients (Data from USDA National Nutrient Database for Standard Reference). The difficulty might be to harmonize the formats of the ingredients between the two datasets.

## Challenges 
* How to merge datasets with very different identifiers (e.g. “BROCCOLI/CAULIFLOWER,CAULIFLOWER WHOLE” vs “broccoli, raw”)?

## Limitations of the dataset 
* No time/location indications —> This might bring up limitations in the ability to reason about the awareness of househoulds regarding their meat consumption as this concern/trend is a rather recent one.
* Different identifiers to same concepts —> how to merge?
* Demographic data only on 800 households, income very broadly categorized —> potentially reducing the size of the dataset 

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







