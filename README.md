# Amazon_Vine_Analysis

## Overview

This project involved analyzing [Amazon](https://www.amazon.com/) reviews written by members of the paid [Amazon Vine program](https://www.amazon.com/vine/about). The Amazon Vine program is a service that allows suppliers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review. Of fifty datasets, we went with video games to avoid conflict of interest (Jaime Starling sells multiple products to Amazon, but not video games). From there we extracted, transformed, and loaded the data for analysis, to see if there is any bias towards favorable reviews from Vine members. 

## The Dataset for Products

The video game review dataset comes from Amazon's [AWS](https://aws.amazon.com/) is quite large and can be opened [here](https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Video_Games_v1_00.tsv.gz) but not necessary as this dataset needed to be extracted and transformed for the analysis. 
- Duplicate lines of product were removed and dates were reformatted to look the same. 
- This gave us a count of 65,792 individual products in the video game category. 
- Tables of the cleaned data failed to load into another software to show results but were not necessary for the analysis. 

## The Dataset for Vine Reviews

The same video game review dataset was extracted again and transformed to show only products with 20 or more reviews and deemed "helpful" by at least 50% of other customers, giving us 40,565 reviews to analyze. We separated the reviews that were Vine participants from those that were not. Only 94 reviews were from Vine participants, the remaining 40,471 were not.

