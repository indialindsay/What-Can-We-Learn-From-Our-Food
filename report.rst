.. code:: ipython3

    from IPython.display import Image, display

**Taking A Quick Look At hte Nutritional Content of Products**

Let’s figure out which countries offer the healthiest products. Though
there are many schools of thought when it comes to evaluating nutrition
labels, one should typically avoid foods high in sugar, saturated and
trans fats, and sodium while foods high in protein and fiber are
considered healthy to eat.

.. code:: ipython3

    display(Image(filename='fig1.png'))



.. image:: output_2_0.png


Sugar has fairly detrimental affects on health. It can lead to weight
gain, increased risk of type 2 Diabetes, food addictions, and chronic
digestive issues. Saturated and trans fats can causes increases in
harmful LDL cholesterol levels, create inflammation, and contribute to
insulin resistance. Excess sodium can lead to elevated blood pressure
and cause varying health problems.

Italy clearly takes home the gold when it comes to average sugar and fat
content while Australia is the runner-up in terms of sodium. In general,
most countries products tend to be fairly high in sugar.

Protein is essential within a diet as it is used by our bodies to build
and repair tissues. Our body is unable to store protein and needs
relatively large quantities of it. Fiber aids our bodies in regulating
digestion and lowers cholesterol levels. It is recommended to eat foods
high in fiber to help achieve a healthy weight.

From the above plots, we observe that Switzerland offers products with
the highest average protein content while Australia’s products have the
highest average fiber content.

**Which Country Offers the Healthiest Food Items?**

Let’s see which country offers products with the greatest amount of
protein and fiber per 100g.

.. code:: ipython3

    display(Image(filename='fig2.png'))



.. image:: output_5_0.png


It seems a little odd that the US has a product with a 100g of protein
and another with 100g fiber … for a product to have 100 grams of protein
or fiber per 100 grams, it must be entirely made up of protein or fiber.
Let’s see what these products are.

.. code:: ipython3

    display(Image(filename='fig3.jpg'))



.. image:: output_7_0.jpg


Unless the Tcho-A-Day Dark Chocolate bar actually is made of pure
protein (if so, please tell me where to find it 😋), its protein content
is probably the result of a data entry error. Otherwise, unflavored
gelatin (a protein product derived from collagen) takes the gold for the
US. This product is typically 99% protein and often taken as a protein
supplement.

.. code:: ipython3

    display(Image(filename='fig4.jpg'))



.. image:: output_9_0.jpg


The products the US offers with the highest fiber content are all a
little unusual. Agar-agar is a jelly-like product derived from seaweed.
Guar gum consist of the fiber from the seed of the guar plant and
Xantham gum is a plant-based thickening and stabilizing agent. All three
of these products are typically used as thickening or stablizing agents
within vegan cooking to help food imitate the consistency or creamyness
provided from using animal products. These products may indicate that a
market for vegan, animal-product substitutes exists in the US.

While we’re on the topic of vegan products…

**Let’s Look At The Popularity of Alternative Diets By Country**

If a product fits a vegetarian diet, than it contains no animal meat
products. If it fits a vegan diet, it contains no animal or dairy
products. Foods that are vegan are also vegetarian. If a food product is
vegan/vegetarian, it is recorded in the product’s label column. If a
product has meat and/or dairy products, it is recorded in the categories
column.

The following code grabs the appropriate tag.

Some food items lack information on their categories or labels. If this
is case, the product’s special diet will be labeled as ‘Not Specified’.
We will exclude these products from our analysis.

.. code:: ipython3

    display(Image(filename='fig5.png'))



.. image:: output_11_0.png


Wow! The majority of Spain’s products in this dataset are vegan and no
other country comes close. All of the countries seem to have fairly high
proportions of dairy products with Russia taking the lead. France offers
the greatest proportion of meat products while the UK and Australia are
tied for the number of vegetarian products.

*Remember that any vegan products can also be classified as vegetarian.
We chose to separate them here to see how countries differ in products
offered between these two categories.*

**Does The Nutritional Content of Products Differ By Special Diet
Category?**

.. code:: ipython3

    display(Image(filename='fig6.png'))



.. image:: output_13_0.png


Meat products generally have high average values of protein, fat, and
sodium while vegetarian and vegan products take the lead in average
fiber content.

All types of diets tend to be fairly high in fat, let’s take a closer
look at how the type of fat differs by diet. Remember, bad fat per 100
grams measures the total amount of both saturated and trans fats per 100
grams in the product

.. code:: ipython3

    display(Image(filename='fig7.png'))



.. image:: output_15_0.png


It looks like the fat content of dairy products is primarily derived
from the unhealthy types of fats. Vegan and vegetarian tend to have
lower values of bad fats per fat content while overall, meat products
tend to be fairly low in fat.

**How Does The Carbon Footprint Differ By Country?**

.. code:: ipython3

    display(Image(filename='fig8.png'))



.. image:: output_17_0.png


France and Switzerland are the only countries to provide information on
the carbon footprint of their products. Their products have about the
same mean carbon footprint.

**What Nutrients Are Related To Carbon Footprint?**

.. code:: ipython3

    display(Image(filename='fig9.png'))



.. image:: output_19_0.png


It looks like there’s a fairly strong positive relationship between a
product’s carbon footprint and the amount of protein and sodium it
contains.

Let’s look into the category tags of these products by country using a
word cloud.

**Categories: Switzerland**

.. code:: ipython3

    display(Image(filename='fig10.png'))



.. image:: output_22_0.png


**Categories: France**

.. code:: ipython3

    display(Image(filename='fig11.png'))



.. image:: output_24_0.png


From Switzerland’s word cloud, you can tell their popular products are
dairy, yogurt, chocolate, sugary snack’s and plant based foods. France
also has a number of plant based products, chocolate, and sugary snacks
while differing from Switzerland in the popularity of non-sugar
beverages and cereal products. Compared to Switzerland, France has both
a greater number of products in this dataset and a greater variety of
popular product categories.

**Concluding Thoughts**

We found that Italy may have a bit of a sweet tooth, offering products
that tend to have the highest average amounts of sugar and bad-fats per
100 grams. Australia’s products contain the highest average amounts of
sodium and fiber. Given the sodium content tends to be higher in
packaged goods, this could imply that Australia eats more processed and
packaged food than other countries. Australia also offers a high
proportion of vegetarian products, which tend to have high fiber
content. When combined with the fact that Australia’s products contained
the highest average amounts of fiber, this may indicate a strong
preference of vegetarian food items in Australia.

Switzerland and France are the only countries that record the
carbon-footprint of their products, suggesting a more environmentally
conscious population. They both intersect in their preference for
chocolate, sugary snacks, and plant-based products. Switzerland’s food
items boast the highest average protein value while also offering many
dairy and yogurt products. France offers the greatest proportion of meat
products while non-sugar beverages and cereal products are quite
popular.

While the US may not have had the highest averages for specific
nutrients, they offer products with the most extreme amounts of protein
and fiber. This may imply the existence of a health conscious market
within the US, focused on taking supplements or food products merely for
their nutritional value.

Spain earns the gold medal when it comes to the amount of vegan products
offered. This may suggest the existence of a large market for
plant-based, meat alternatives.

Overall, it is important to remember the that insights in this dataset
reflect the products uploaded to the open food facts database. The data
offers interesting tidbits about the ways different countries eat
however, it may not be representative of the general eating habits of
the whole population of these countries.
