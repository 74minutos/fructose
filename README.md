# fructose checker
I've created a 'fructose checker' to be presented on google datastudio. [Here's the result](https://datastudio.google.com/s/r98IWdhnfHU)

The source for all this graphs is Nuttab database: [Australian Food Composition Database](https://www.foodstandards.gov.au/science/monitoringnutrients/afcd/Pages/downloadableexcelfiles.aspx)

I've treated all the data through google sheets, because of two main reasons:
* I want something easy to manipulate and with direct integration with Datastudio
* There are some interesting functions that I needed from google sheets (such as googletranslate or the Wikipedia plugin)

I cleaned a little bit the document to my purposes and voilà. Now that he have the data well structured is time to do the research. As I've been learning through the past of time, there are plenty of variables to have in mind when it comes to fructose malabsorption, so I've tried to condense the main ones in this dashboard. These are the variables and the rules that I've followed.:
1. Fructose amount. Of course, the main indicator that we always have to check is the total amount fo fructose. If the amount of one food is higher to 15, the box will appear as orange, saying that this is not recommedable for consumption. If not, we can continue in our journey.
2. Fructose-glucose diff: There are tons of scientific evidence that glucose helps to absorb the excess of fructose, so I've created a "calculator" of that difference to have another variable to count on. If the total amount of this difference is below 2 it will be considered as valid for consumptio, but if the amount of fructose is very high it doesn't matter the glucose amount. Among many others, these are the main articles where you can find that evidence:
 
⋅⋅⋅2a. [Intestinal fructose transport and malabsorption in humans](https://journals.physiology.org/doi/full/10.1152/ajpgi.00457.2010)
⋅⋅⋅2b. [Fructose Malabsorption](https://en.wikipedia.org/wiki/Fructose_malabsorption)
⋅⋅⋅2c. [Dietary fructose and gastrointestinal symptoms: a review](https://pubmed.ncbi.nlm.nih.gov/15447771/)
⋅⋅⋅2d. [Fructose Malabsorption and Symptoms of Irritable Bowel Syndrome: Guidelines for Effective Dietary Management](http://sacfs.asn.au/download/SueShepherd_sarticle.pdf)
⋅⋅⋅2e. I use this one to stablish the maximum difference tolrate in the checker: [Dietary fructose intolerance, fructan intolerance and FODMAPs](https://pubmed.ncbi.nlm.nih.gov/24357350/)

3. Of course, if you have fructose malabsorption for sure you know that all sugars are *no good*. For that reason I've created the third step, in which we can evalute the total sugars that the food is containing.
