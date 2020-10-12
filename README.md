# What-Can-We-Learn-From-Our-Food

The dataset I analyze was obtained from Open Food Facts (https://world.openfoodfacts.org/) - a free collaborative database of food products. Each product is uploaded by users who scan the food products and their nutrition labels. 

The dataset originally contained information on 356,027 food products from 224 different countries with 163 characteristics for each product. For my analysis, I wanted to use an organized and condensed dataset. __Check out how I cleaned and inspecting the [data quality here](https://github.com/indialindsay/What-Can-We-Learn-From-Our-Food/blob/master/Data%20Quality.ipynb)__, controlling for missing data, errors due to data input inconsistencies, narrowed down extraneous columns, and classified products into a common diet type. 

The cleaned dataset contained 352433 and 33 columns. Out of these columns, there are several key variables of interest.

The country column will tell us the country in which this product was uploaded to the food products database. We will rely on it as an indicator of the country the food product is associated with. Product_name serves as an identifier for each product.

I will rely on the following columns to analyze the general nutrition characteristics of the food products:
- Saturated-Fat 
- Trans-Fat
- Fiber
- Sugars
- Proteins
- Sodium 

The Categories and Labels columns will help us identify which type of diet the food product falls into. Though the carbon footprint column has many missing values, we will still use it to learn what we can about the environmental impact of products. We also have a column 'Special Diet' that indicates whether the food product can be classified into a common diet type. 

## [Click here](https://github.com/indialindsay/What-Can-We-Learn-From-Our-Food/blob/master/Exploring%20Nutrition%20By%20Country.ipynb) to explore how health quality of countries differs based upon their food products.

