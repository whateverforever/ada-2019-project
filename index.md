<h1>Can marketing help us being vegetarian?</h1>
<h2>A societal study identifying meat consumption patterns</h2>

>Climate change is no longer some far-off problem; it is happening here, it is happening now.
> -- <cite>[Barack Obama][1]</cite>

[1]:https://www.weforum.org/agenda/2015/11/15-quotes-on-climate-change-by-world-leaders/

...affecting our planet and our society. Hence, it is time to take the relevant steps to avoid the worst impacts of it. This concerns various dimensions, such as renewable energy, emissions and agriculture. Most importantly however is to note, that each of us is able to fight climate change. It starts off with a very simple issue: our **food consumption**. Dietary changes towards healthier diets can help to reduce the environmental impacts of the food system, in particular with regard to animal products, when they are replaced by less intensive food types [[Nature]](https://www.nature.com/articles/s41586-018-0594-0). This form of _human diet_ can actively promote a change in the amount of greenhouse-gas emissions [[Nature 572, 291-292 (2019)](https://www.nature.com/articles/d41586-019-02409-7)].

Since this project's overall goal is **"Data Science for the good"**, an analysis of our daily consumption of everyday commodity products taken from Household Transactional Data offers the potential to reveal patterns and latent structures and relations in the interaction of marketing and transaction behavior on meat and vegetarian products. With transactions from more than 2500 households from different societal status over 2 years the data set "[Dunnhumby - The complete journey](https://www.dunnhumby.com/careers/engineering/sourcefiles)", used in this analysis, offers the chance to link societal status, income and living constellations to a topic which gains more and more importance **our meat consumption**. 

Knowledge about interdependencies and drivers of customer preferences and behaviors is a crucial factor for effective customer-based strategies. Having these insights at hand, it might be possible to develop new strategies to actively take influence on improving awareness for meat consumption via more precisely targeted advertisements and promotions, satisfying both the customer himself, as well as the retail industry. For instance, a correlation of households with lower income households exhibiting a less balanced/more meat-focused food could be dispersed by placing well-suited advertisements for more vegetarian food.

## Demographic landscape of the households in the data set
<!-- <iframe id="igraph" scrolling="no" style="border:none;" seamless="seamless" src="test.html" height="525" width="100%"></iframe> -->
This data set contains 2500 households who are frequent shoppers at a retailer. It contains all of each household's purchases from a diverse number of categories (not only food-related). For certain households (801 out of 2500), also demographic information, as well as direct marketing contact history was included. This covers at least one third of the population to gain an overview of the demographic landscape of the corresponding data set. 

First looking at the age ranges, the biggest share (~35%) of households covers a range of 45-54 years, followed by a range of 35-44 (~25%). The smallest share is represented by the 19-24 years range, corresponding in most cases to Single Households. It can be further inferred that most of the 801 households are married or at least in partnership, which split up in nearly equally sized subgroups of having children and not having children. The third group in the marital categorization is includes Single households. It includes households from all age ranges. 


## Consumption Behaviour

Are there differences in the meat consumption between incomes? Do people with a higher income eat more or less week per? To find out, we calculate the weight of meat, bought per household and normalize this by the number of people in the household, and the duration of data-collection for this household.

Let's look at a plot of the different income groups we have. To be able to actually say anything about the data, we also plot the 95% confidence interval.

![Meat consumption per day and income](images/demographics_meat_weight-income.png)

We notice a few things: Lower income people with an income of less than 15K per year tend to buy more meat that people that earn between 75-149K. On the one hand, this seems counter-intuitive, since meat can be very expensive. On the other hand, nowadays many cheap meat products from factory farming exist. 

<div style="background-color:orange; width:100%; padding:20px; color:black;">Include average prices of meat and other shit</div>

Another interesting observation is that the lowest meat consumption comes from the high-income bracket of 200-249K. The consumption is significantly lower than of the beforementioned income brackets.

It seems there is an inverse relation between the income people have and their meat consumption. Possible explanations might be that higher income people buy less food in general...

<div style="background-color:orange; width:100%; padding:20px; color:black;">Can we check this?</div>

... or that they are more conscious about their food choices, buying for example fewer, but higher quality meats.

<div style="background-color:orange; width:100%; padding:20px; color:black;">Can we check this?</div>

Meat consumption is way less clear for the different age categories. In fact we can't say there is any significant difference between the age groups.

<div style="background-color:orange; width:100%; padding:20px; color:black;">Run a test for this explicitly?</div>

![Meat consumption per day and, grouped byage](images/demographics_meat_weight-age.png)

It is different for the marital status, as we can see that households of married couples eat way less meat than single person households or households were the data doesn't specify. This might be due to healthier food choices made by parents, which are more likely to occur in married households. Unfortunately, this can't be answered with confidence, due to the dataset not having detailed enough information about the number of kids.

![Meat consumption per day and, grouped by marital status](images/demographics_meat_weight-married.png)

However, if we regroup the existing data we have about adults without kids and kids vs singles, we can still see some amusing differences.


## Campaign and what kind of food they promote

### The Role of Coupons

Marketing plays a big role in people's grocery shopping behaviour. Are people directed to buy meat and fish? To take a look at that we observe two marketing aspects: Campaigns which distribute coupons and advertisment.

We first look at the coupons distributed by the 30 campaigns. To get an vague idea of the campaigns, we look at how many coupons they distribute and at how many coupons are actually redeemed.

<iframe id="igraph" scrolling="no" style="border:none;" seamless="seamless" src="data/campaign_overview.html" height="525" width="100%"></iframe>

We can see that the coupons do have an impact, since many of them actually get redeemed. In fact, around 86% of distributed coupons are getting redeemed. If we consider that the campaigns, and with them the coupons, are being designed by someone, we see that there is a strong influence on the buying actions of customers though the coupons.

With that in mind, let's take a closer look at the coupons and what food categories are promoted.

<iframe id="igraph" scrolling="no" style="border:none;" seamless="seamless" src="data/Campaign_proportion_food.html" height="525" width="100%"></iframe>

Feel free to explore what kind of food items are being promoted by the campaigns. When you're ready, continue on to find out what part meat and fish play in the campaigns.

### Promotions for Meat and Fish

![proportion of coupon distributed per category for each campaign](data/campaign_veg.png)

The campaign individual shares of meat or fish related coupons are mostly low. Furthermore, vegetarian products seem to be promoted more. Also worth looking into is to see how many of the distributed coupons are redeemed in the end.

![proportion of coupon redeemed per category for each campaign](data/campaign_veg_re.png)

The proportions of distributed and redeemed coupons are quite similar. Thus, the usage rate of meat and fish coupons and vegetarian coupons are comparable aswell. Testing if there is a difference between vegetarian and non-vegetarian coupons, we find that there actually are significantly (95% CI) more coupons distributed for vegetarian than non-vegetarian products.

<div style="background-color:orange; width:100%; padding:20px; color:black;">Either remove right hand side plot, or write in text, that we can't say anything about the difference in redemption</div>


![](images/veg-nonveg-coupons.png)

We can draw the conclusion that campaigns do not direct people to buy non-vegetarian food. Quite the opposite, it seems like more effort is spent on trying to sell non-meat and non-fish coupons!

---

Next, we look at the other marketing aspect: advertisement. Coupons are only half the story when the influence of the campaigns is concerned. The campaigns also distribute leaflets advertising different items. These ads can be in different parts of the leaflet. So how are the different food categories advertised?

<iframe id="igraph" scrolling="no" style="border:none;" seamless="seamless" src="data/ad_types.html" height="525" width="100%"></iframe>

The best postition in a magazine is certainly the front page. Approximately 15% of all meat and only 1% of the fish products are advertised on the frontpage. On the other hand, vegetarian animal product are in 30% of the time are displayed on the frontpage. The numbers for vegetables and fruits are 10% and 7% respectively. Again, it does not appear that meat or fish is particularly advertised.

In conclusion, we can say that it seems like marketing does not promote meat and fish consumption, but instead does so for vegetarian products.

## How do consumers react to those campaigns?
