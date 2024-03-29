# Latent structures in Household Transactional Data — A societal study identifying meat consumption patterns

> File with analysis: `data_analysis.ipynb`

> [Final Data Story](https://brudermueller.github.io/ada-2019-project/)


# Abstract
> A 150 word description of the project idea, goals, dataset used. What story you would like to tell and why? What's the motivation behind your project?

The consumption of everyday commodity products offers the potential to reveal societal inequalities, as well as to identify social milieus including their habits and behaviors. With transactions from more than 2500 households from different societal status over 2 years we try to identify hidden relationships and patterns. This project work will focus on two consecutive interwined aspects: societal latent structures in consumption and transaction behavior and vegetarianism.

This dataset offers the chance to link societal status, income and living constellations to a topic which gains more and more importance in recent times with growing concerns in **climate change: our meat consumption**. This form of _human diet_ can actively promote a change in the amount of greenhouse-gas emissions [[Nature 572, 291-292 (2019)](https://www.nature.com/articles/d41586-019-02409-7)].

Knowledge about interdependencies and drivers of customer preferences and behaviors is a crucial factor for effective customer-based strategies. With this knowlegde at hand, it might be possible to develop new strategies to actively take influence on improving awareness for meat consumption via more precisely targeted advertisements and promotions, satisfying both the customer himself, as well as the retail industry. For instance, the assumed correlation of households with lower income households exhibiting a less balanced/more meat-focused food could be dispersed by placing well-suited advertisements for more vegetarian food.

# Research questions
> A list of research questions you would like to address during the project. 

## Societal Analysis
* **Do the food consumption patterns/habits reflect the belonging to a social class?**
  * Do lower income people rely on coupons? If so, are there food choices steered by the available coupons (vegetarian vs non-veg for instance)? —> Responsibility of Shops? Education?
* **What kind of products are promoted?** 
  * Does the advertising industry push our society towards “bad habits”?

## Vegetarianism
* **What is the proportion of vegetarian products in the total household spendings? (i.e. how much money is spent on healthy foods?)**
    * Do single-person households consume less meat than families (avg. per person)? 

## Marketing strategies
* **Identify clusters with Customer Segmentation**
    * Identify groups/clusters of customers differing in product interest/market participation/response to marketing — come up with potential recommendations for retail (wrt. product placement, promotional efforts, etc.) 


# Dataset
> List the dataset(s) you want to use, and some ideas on how do you expect to get, manage, process and enrich it/them. Show us you've read the docs and some examples, and you've a clear idea on what to expect. Discuss data size and format if relevant.

* [Dunnhumby - The complete journey](https://www.dunnhumby.com/careers/engineering/sourcefiles): provides insights of the household transactions of 2500 households over 2 years (collected by Data Science Company Dunnhumby)

## Contents of the dataset
* socioeconomical status of 800 households (income, marital status, number of kids)
* list of 30 campaigns with list of coupons distributed and redeemed 
* list of advertisements of the products and their display in the stores
* list of the transactions (with sales value, transaction time, quantity, various types of discount)
* list of products (with various categories)

## Challenge
Group products in a few categories such as meat, fish, vegetables to be able to extract informations on meat consumption or vegetarianism in general.

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

# Milestone 3 — next steps

* *Campaign and coupons analysis:* continue our analysis on how retailers promote different categories of food and how people respond to it. In practice, this means for instance combining what has already been done with the transactions to find out how much people save money thanks to these campaigns and if it differs from one category of food to another.

* *Household behaviour:* continue our analysis on the demographics in order to find different behaviour (due to income or type of family) towards meat consumption and vegetarianism in general.

* *Advertisement analysis:* continue analysis (look at both distribution of ads within one category of food and across all categories, which ones get more ads in the best displays) and combine results with campaign and coupons analysis.

Ultimately, our goal would be to combine more and more our results in order to get a precise understanding of both retailers and consumers towards meat consumption and vegetarianism in general.


---
# Contributions of Group Members

| Member | Contribution |
| ----- | ------ |
| Thanh  | Design of the products categories, plot of the interactive plots for the datastory |
| Giacomo | Exploratory analysis, Detailed Campaign analysis, Detailed statistical tests |
| Max |  Exploratory analysis towards meat consumption of different groups, write the datastory |
| Lara | Review and refinements of the entire analysis, write the datastory | 
| *All* | Final Presentation, Writing up the report |









