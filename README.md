# Amazon_Vine_Analysis

## Overview of Analysis 
SellBy is a start-up company that is looking into utilizing Amazon Vine. A company can pay a small view to Amazon and provide products to Amazon Vine membres, who are then required to publish a review. This project was to analyze Amazon reviews written by members of the paid Amazon Vine Program. The dataset that was reviewed in this analysis was baby products. PySpark was then used to extract, transform and load the date. Our goal of the analysis is to determine if there is any bias toward favorable reviews from Vine members in the dataset. 

## Results 
An initial "vine" dataframe was created that held all of the information we would need to conduct our analysis. We then filtered the data to retrieve all rows where the total vote count was greater than or equal to 20. This allowed us to pick reviews that are more likelty to be helpful. 

![image](https://user-images.githubusercontent.com/117782103/225980501-427e4f4e-b6b4-492f-b4fd-8890b34506b1.png)

Next we took that total vote dataframe and retrieved all rows where the number of helpful votes divded by the total votes was greater than or equal to 50%. 

![image](https://user-images.githubusercontent.com/117782103/225980627-b3f38813-1e9b-4d22-ab46-318c90545c1f.png)

Then we created another dataframe to retrieve all the rows where a review was written as part of the Vine program, meaning they were paid to write the review. 

![image](https://user-images.githubusercontent.com/117782103/225980726-a9c300a6-8738-45b2-8eed-77c7704f462e.png)

Lastly, we retrieved the rows where a review was written that was not part of the Vine program, meaning the review not paid. 

![image](https://user-images.githubusercontent.com/117782103/225980797-dc7f5500-05ca-45e9-9cdf-b1797405cd94.png)

Using these dataframes, we were ready to dive deeper into our anlaysis to answer a few key questions to determine if bias occurs on Vine reviews. 

### How many Vine reviews and non-Vine reviews were there?

For the dataset on baby products, there were 5,028 reviews written as part of the Vine program (paid) and 495,942 reviews written that were not part of the Vine program (unpaid).

![image](https://user-images.githubusercontent.com/117782103/225980867-c7d28fe6-7d04-439f-ba6c-3cf2be07a74a.png)

### How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

Looking at the reviews that were paid from Vine, there were 2,368 reviews that were given 5 starts. In comparison, the unpaid or non-Vine reviews, had 265,843 5 start reviews. 

![image](https://user-images.githubusercontent.com/117782103/225980929-fda7cad9-524e-4f00-9e81-9f4406bdd0e8.png)

### What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

To put this in perspective we took the total number of five start reviews and divided it by the total reviews. For the paid Vine programs 47.1% of the reviews written were 5 stars. Unapid reviews resulted in 53.5% of the reviews being 5 stars. 

![image](https://user-images.githubusercontent.com/117782103/225980998-834e1409-f84b-4bbe-af6b-7f323af2b365.png)

## Summary 

According to the results that were analyzed in the baby product category, there is not positivity bias for reviews in the Vine program. This could be different based on the type of products being reviewed. However, for baby products, 47.1% of all the reviews written were 5 stars. This is in comparison to the 53.5% of 5 star reviews that were written for reviews that were not associated with the Vine program. Since this percentage is higher, that would tell us that there is no positivity bias as part of the program. 

### Additional Analysis 

One additional analysis that could be performed to support this statement is
