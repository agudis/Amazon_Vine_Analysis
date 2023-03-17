# Amazon_Vine_Analysis

## Overview of Analysis 
SellBy is a start-up company that is looking into utilizing Amazon Vine. A company can pay a small view to Amazon and provide products to Amazon Vine membres, who are then required to publish a review. This project was to analyze Amazon reviews written by members of the paid Amazon Vine Program. The dataset that was reviewed in this analysis was baby products. PySpark was then used to extract, transform and load the date. Our goal of the analysis is to determine if there is any bias toward favorable reviews from Vine members in the dataset. 

## Results 
This image below shows what our vine dataframe was filtered for. 

![image](https://user-images.githubusercontent.com/117782103/225980315-4d5e13ec-79fa-49af-9c25-03f2e52d0af3.png)

![image](https://user-images.githubusercontent.com/117782103/225980501-427e4f4e-b6b4-492f-b4fd-8890b34506b1.png)

![image](https://user-images.githubusercontent.com/117782103/225980627-b3f38813-1e9b-4d22-ab46-318c90545c1f.png)

![image](https://user-images.githubusercontent.com/117782103/225980726-a9c300a6-8738-45b2-8eed-77c7704f462e.png)

![image](https://user-images.githubusercontent.com/117782103/225980797-dc7f5500-05ca-45e9-9cdf-b1797405cd94.png)


### How many Vine reviews and non-Vine reviews were there?
For the dataset on baby products 

![image](https://user-images.githubusercontent.com/117782103/225980867-c7d28fe6-7d04-439f-ba6c-3cf2be07a74a.png)


### How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

![image](https://user-images.githubusercontent.com/117782103/225980929-fda7cad9-524e-4f00-9e81-9f4406bdd0e8.png)


### What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

![image](https://user-images.githubusercontent.com/117782103/225980998-834e1409-f84b-4bbe-af6b-7f323af2b365.png)


## Summary 

### Additional Analysis 
