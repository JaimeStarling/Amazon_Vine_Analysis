# Amazon_Vine_Analysis

## Overview

This project involved analyzing [Amazon](https://www.amazon.com/) reviews written by members of the paid [Amazon Vine program](https://www.amazon.com/vine/about). The Amazon Vine program is a service that allows suppliers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review. Of fifty datasets, we went with video games to avoid conflict of interest (Jaime Starling sells multiple products to Amazon, but not video games). From there we extracted, transformed, and loaded the data for analysis, to see if there is any bias towards favorable reviews from Vine members. 

## The Dataset for Products

The video game review dataset comes from Amazon's [AWS](https://aws.amazon.com/) is quite large and can be opened [here](https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Video_Games_v1_00.tsv.gz) but not necessary as this dataset needed to be extracted and transformed for the analysis. 
- Duplicate lines of product were removed and dates were reformatted to look the same. 
- This gave us a count of 65,792 individual products in the video game category. 
- Tables of the cleaned data failed to load into another software to show results but were not necessary for the analysis. 

## The Dataset for Vine Reviews

The same video game review dataset was extracted again and transformed to show only products with 20 or more reviews and deemed "helpful" by at least 50 percent of other customers.
- This gave us 40,565 reviews to analyze. 
- Only 94 reviews were from Vine participants, less than 1 percent of total reviews.
- The remaining 40,471 were not from Vine participants.

## Results for Analysis

The highest review possible at Amazon is a "5-Star" and has even determined what is displayed at Amazon's [physical locations](https://www.amazon.com/find-your-store/b/?node=17608448011). A simple chart with totals and percentages below

![This is an image](https://github.com/JaimeStarling/Amazon_Vine_Analysis/blob/main/Del_2_Images/tablefromdel2.png)

shows that of the transformed dataset, 39 percent of the reviews by non-Vine participants were "5-Star." However, the majority (only just!) of reviews by Vine participants were "5-Star." 

## Summary

In politics, a vote of 51 percent is a "mandate," and Amazon algorithms are run on millions of tiny elections for their [350 million](https://www.bigcommerce.com/blog/amazon-statistics/#amazon-everything-to-everybody) products. Participation in the Vine program, for the cost of product, shipping, and any fees, is a decent investment for increasing customer review results, which Amazon suppliers know to "feed the beast" algorithm of showcasing your product.



