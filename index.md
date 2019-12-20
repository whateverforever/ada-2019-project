<header>
  <h1>Can marketing help us being vegetarian?</h1>
  <h2>A societal study identifying meat consumption patterns</p>
</header>


>Climate change is no longer some far-off problem; it is happening here, it is happening now.
> -- <cite>[Barack Obama][1]</cite>

[1]:https://www.weforum.org/agenda/2015/11/15-quotes-on-climate-change-by-world-leaders/

...affecting our planet and our society. Hence, it is time to take the relevant steps to avoid the worst impacts of it. This concerns various dimensions, such as renewable energy, emissions and agriculture. Most importantly however is to note, that each of us is able to fight climate change. It starts off with a very simple issue: our **food consumption**. Dietary changes towards healthier diets can help to reduce the environmental impacts of the food system, in particular with regard to animal products, when they are replaced by less intensive food types [[Nature]](https://www.nature.com/articles/s41586-018-0594-0). This form of _human diet_ can actively promote a change in the amount of greenhouse-gas emissions [[Nature 572, 291-292 (2019)](https://www.nature.com/articles/d41586-019-02409-7)].

Since this project's overall goal is **"Data Science for the good"**, an analysis of our daily consumption of everyday commodity products taken from Household Transactional Data offers the potential to reveal patterns and latent structures and relations in the interaction of marketing and transaction behavior on meat and vegetarian products. With transactions from more than 2500 households from different societal status over 2 years the data set "[Dunnhumby - The complete journey](https://www.dunnhumby.com/careers/engineering/sourcefiles)", used in this analysis, offers the chance to link societal status, income and living constellations to a topic which gains more and more importance **our meat consumption**. 

Knowledge about interdependencies and drivers of customer preferences and behaviors is a crucial factor for effective customer-based strategies. Having these insights at hand, it might be possible to develop new strategies to actively take influence on improving awareness for meat consumption via more precisely targeted advertisements and promotions, satisfying both the customer himself, as well as the retail industry. For instance, a correlation of households with lower income households exhibiting a less balanced/more meat-focused food could be dispersed by placing well-suited advertisements for more vegetarian food.

## What kind of househould do we observe?
<iframe id="igraph" scrolling="no" style="border:none;" seamless="seamless" src="test.html" height="525" width="100%"></iframe>

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

It is different for the marital status, as we can see that households of married couples eat way less meat than single person households or households were the data doesn't specify. This might be due to healthier food choices made by parents, which are more likely to occur in married households.

<div style="background-color:orange; width:100%; padding:20px; color:black;">Check this hypothesis (are there more kids in married households)!</div>

![Meat consumption per day and, grouped byage](images/demographics_meat_weight-married.png)

## Campaign and what kind of food they promote

## How do consumers react to those campaigns?
