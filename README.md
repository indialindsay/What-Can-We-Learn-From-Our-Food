## Are there significant differences in the general products countries eat?

The dataset I analyze was obtained from Open Food Facts (https://world.openfoodfacts.org/) - a free collaborative database of food products. Each product is uploaded by users who scan the food products and their nutrition labels. 

The dataset originally contained information on 356,027 food products from 224 different countries with 163 characteristics for each product. For my analysis, I wanted to use an organized and condensed dataset. __Check out how I cleaned and inspecting the [data quality here](https://github.com/indialindsay/What-Can-We-Learn-From-Our-Food/blob/master/Data%20Quality.ipynb)__

### How many products were uploaded from countries that have at least 1000 products listed?
![plot1](https://user-images.githubusercontent.com/68126147/97117010-1e75a580-16cf-11eb-94b9-fd1c96b9374a.png)

The US and France definitely dominate this dataset. 

### Does the general nutrition content of the food products differ by country? 

Let's try to figure out which countries offer the healthiest products. Though there are many schools of thought when it comes to evaluating nutrition labels, one should typically avoid foods high in sugar, saturated, and sodium. Foods high in protein and fiber are considered healthy to eat.

![plot3](https://user-images.githubusercontent.com/68126147/97829756-996f2b00-1c90-11eb-8ceb-5023969629cc.png)
![plot2](https://user-images.githubusercontent.com/68126147/97829757-996f2b00-1c90-11eb-8276-df13c7475454.png)
 
Sugar has fairly detrimental affects on health. It can lead to weight gain, increased risk of type 2 Diabetes, food addictions, and chronic digestive issues [learn more](https://www.webmd.com/diabetes/features/how-sugar-affects-your-body). Saturated fats can causes increases in harmful LDL cholesterol levels, create inflammation, and contribute to insulin resistance [learn more](https://www.heart.org/en/healthy-living/healthy-eating/eat-smart/fats/saturated-fats). Excess sodium can lead to elevated blood pressure and cause varying health problems. 

Protein is essential within a diet as it is used by our bodies to build and repair tissues. Our body is unable to store protein and needs relatively large quantities of it. Fiber aids our bodies in regulating digestion and lowers cholesterol levels. It is recommended to eat foods high in fiber to help achieve a healthy weight 
[learn more](https://www.mayoclinic.org/healthy-lifestyle/nutrition-and-healthy-eating/in-depth/fiber/art-20043983). 

In general, most countries products tend to have a fairly high average sugar content per product with the US, Canada, and Belgium taking the lead. Russia has both the highest average protein and saturated fat content per 100g. 


### Let's Look At The Popularity of Alternative Diets By Country¶
If a product fits a vegetarian diet, than it contains no animal meat products. If it fits a vegan diet, it contains no animal or dairy products. Foods that are vegan are also vegetarian.

In the data quality file, I used categorized the foods by their diet type. Let's use these tags to discovery which countries have preferences for the different diets.

![plot5](https://user-images.githubusercontent.com/68126147/97829766-9aa05800-1c90-11eb-8e94-1cefe847aa8a.png)

The majority of Spain's products in this dataset are vegetarian and no other country comes close. Pretty much all of Russia's products in this dataset are meat products. The US, Italy, and Belgium also offer a lot of meat products while Germany, Australia, Spain, and the UK have very few if any meat products. Australia and France consume a notable number of vegan products.  

### Which countries offer the most organic products?

![plot6](https://user-images.githubusercontent.com/68126147/97829765-9aa05800-1c90-11eb-89a5-b7544991e9a2.png)

European countries have the greatest proportion of organic products in this dataset. About 1/3 of all of Germany's products are sourced organically. 

### Do any of the countries share common ingredients in their products? 

The US, France, Switzerland, Germany, and Spain contain the most products in this dataset. Let's look into the top 10 most common ingredients in their products and see which ones are shared between countries. 

![venn4](https://user-images.githubusercontent.com/68126147/97829760-9a07c180-1c90-11eb-91fe-271322fd7b84.png)
![venn3](https://user-images.githubusercontent.com/68126147/97829761-9a07c180-1c90-11eb-87e3-964f2a23d6ae.png)
![venn2](https://user-images.githubusercontent.com/68126147/97829762-9a07c180-1c90-11eb-98ff-f082b093e7ac.png)
![venn1](https://user-images.githubusercontent.com/68126147/97829764-9a07c180-1c90-11eb-966d-78c691df7334.png)

The US and Spain share no common ingredients with the other countries while the Northern European countries (Germany, France, and Switzerland) share a few common ingredients. 

You can view the code behind these plots [here](https://github.com/indialindsay/What-Can-We-Learn-From-Our-Food/blob/master/Exploring%20Nutrition%20By%20Country.ipynb)
