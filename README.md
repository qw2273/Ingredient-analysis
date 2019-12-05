# Skincare Products Ingredients Analysis
[image]

## Why this topic? 
Have you ever thought about what your skincare products contain when you applying them on your face? Have you ever confused by what's the difference between the pricy ones and affordable ones? For these pricy products, is it able to find substitutes with similar ingredients? I believe not only me but also many other skincare products users have raised similar concerns. So this project is here to solve your concerns. 

## Data

The first thing I need is a dataset that contains skincare product information. Unfortunately, there is no such downloadable dataset available online, so I have to get one by myself using web scraping techniques. Among all these websites, I found a website called Beautypedia (Beauty + Wikipedia), according to the website itself promoted - No.1 source of a reliable source for cosmetics and skincare products. I restrained my analysis to only moisturizes and eye cream products only. 

## Data Processing 
After taking a closer look, I found the raw data is messy. It seems brands have different ways to name the same ingredient, and there are some spelling mistakes in there. Thus it is necessary to convert these ingredients in a more standard format before making the analysis. The dictionary I used is downloaded from the CIR website. 

## Data Manipulation
The first step will be tokenizing the list of ingredients in the Ingredients column. After splitting them into tokens, we'll make a binary bag of words. Then we will create a dictionary with the tokens: ingredient_idx.

The next step is making a document-term matrix (DTM). Here each cosmetic product will correspond to a document, and each chemical composition will correspond to a term.

[image] 
