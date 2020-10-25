# What-Can-We-Learn-From-Our-Food

The dataset I analyze was obtained from Open Food Facts (https://world.openfoodfacts.org/) - a free collaborative database of food products. Each product is uploaded by users who scan the food products and their nutrition labels. 

The dataset originally contained information on 356,027 food products from 224 different countries with 163 characteristics for each product. For my analysis, I wanted to use an organized and condensed dataset. __Check out how I cleaned and inspecting the [data quality here](https://github.com/indialindsay/What-Can-We-Learn-From-Our-Food/blob/master/Data%20Quality.ipynb)__

### How many products were uploaded from countries that have at least 1000 products listed?
![plot1](https://user-images.githubusercontent.com/68126147/97117010-1e75a580-16cf-11eb-94b9-fd1c96b9374a.png)

The US and France definitely dominate this dataset. 

Let's try to figure out which countries offer the healthiest products. Though there are many schools of thought when it comes to evaluating nutrition labels, one should typically avoid foods high in sugar, saturated and trans fats (we will label these together as bad fats), and sodium. Foods high in protein and fiber are considered healthy to eat.

![plot2](https://user-images.githubusercontent.com/68126147/97117140-d30fc700-16cf-11eb-89b8-14b1c8a28f19.png)
![plot3](https://user-images.githubusercontent.com/68126147/97117141-d3a85d80-16cf-11eb-930e-faca9c9bd360.png)

Sugar has fairly detrimental affects on health. It can lead to weight gain, increased risk of type 2 Diabetes, food addictions, and chronic digestive issues. Saturated and trans fats can causes increases in harmful LDL cholesterol levels, create inflammation, and contribute to insulin resistance. Excess sodium can lead to elevated blood pressure and cause varying health problems.

Italy clearly takes home the gold when it comes to average sugar and fat content while Australia is the runner-up in terms of sodium. In general, most countries products tend to be fairly high in sugar.

Protein is essential within a diet as it is used by our bodies to build and repair tissues. Our body is unable to store protein and needs relatively large quantities of it. Fiber aids our bodies in regulating digestion and lowers cholesterol levels. It is recommended to eat foods high in fiber to help achieve a healthy weight.

From the above plots, we observe that Switzerland offers products with the highest average protein content while Australia's products have the highest average fiber content.

__Relying upon the country's average score in terms of the above healthy/unhealthy nutrients, Italy provides some of the unhealthiest products while Switzerland, Russia, and Australia offer the healthiest.__

### Let's Look At The Popularity of Alternative Diets By Country¶
If a product fits a vegetarian diet, than it contains no animal meat products. If it fits a vegan diet, it contains no animal or dairy products. Foods that are vegan are also vegetarian.

In the data quality file, I used categorized the foods by their diet type. Let's use these tags to discovery which countries have preferences for the different diets.

![plot5](https://user-images.githubusercontent.com/68126147/97117143-d3a85d80-16cf-11eb-875f-61d72657add2.png)

The majority of Spain's products in this dataset are vegan and no other country comes close. All of the countries seem to have fairly high proportions of dairy products with Russia taking the lead. France offers the greatest proportion of meat products while the UK and Australia are tied for the number of vegetarian products.

*Remember that any vegan products can also be classified as vegetarian. We chose to separate them here to see how countries differ in products offered between these two categories.*

### Does The Nutritional Content of Products Differ By Special Diet Category?
![plot6](https://user-images.githubusercontent.com/68126147/97117144-d3a85d80-16cf-11eb-9b25-843acea5a164.png)

Meat products generally have high average values of protein, fat, and sodium while vegetarian and vegan products take the lead in average fiber content.

All types of diets tend to be fairly high in fat, let's take a closer look at how the type of fat differs by diet. Remember, bad fat per 100 grams measures the total amount of both saturated and trans fats per 100 grams in the product

![plot7](https://user-images.githubusercontent.com/68126147/97117145-d3a85d80-16cf-11eb-9eb4-aa245f55b3d9.png)

It looks like the fat content of dairy products is primarily derived from the unhealthy types of fats. Vegan and vegetarian tend to have lower values of bad fats per fat content while overall, meat products tend to be fairly low in fat.

We found that Italy may have a bit of a sweet tooth, offering products that tend to have the highest average amounts of sugar and bad-fats per 100 grams. Given the majority of fat in dairy products stems from bad-fats, it might be helpful to stress the benefits of low dairy diets.

Australia's products contain the highest average amounts of sodium and fiber. Given the sodium content tends to be higher in packaged goods, this could imply that Australia eats more processed and packaged food than other countries. Australia also offers a high proportion of vegetarian products, which tend to have high fiber content. When combined with the fact that Australia's products contained the highest average amounts of fiber, this may indicate a strong preference of vegetarian food items in Australia.

Spain earns the gold medal when it comes to the amount of vegan products offered. This may suggest the existence of a large market for plant-based, meat alternatives.

You can view the code behind these plots [here](https://github.com/indialindsay/What-Can-We-Learn-From-Our-Food/blob/master/Exploring%20Nutrition%20By%20Country.ipynb)
