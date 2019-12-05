# Skincare Products Ingredients Analysis
[image]

## Why this topic? 
Have you ever thought about what your skincare products contian when you applying them on your face? Have you ever confused by what's the difference between the pricy ones and affordable ones? For these pricy products, is it able to find subsitutes with similar ingredients? I believe not only me, but also many other skincare products users have raise similar concerns. So this project is here to solve your concerns. 

## Data

The first thing I need is a dataset that contains skincare products inforamtion. Unfortunately, there is no such downloadable dataset available online, so I have to get one by myself using web scrapping techniques. Among all these websites, I found a website called Beautypedia (Beauty + Wikipedia), according to website itself promoted - No.1 source of realiable source for cosmetics and skincare products. I restrained my analysis to only moisturze and eyecream products only. 

## Data Processing 
After checking, I found the raw data is really messy. It seems brands have their different ways to name a same ingredient, and there are some spelling mistakes in there. Thus it is necessary to convert these ingredients in a more standard format before making analysis. The dictionary I used is downloaded from CIR website. 

## Data Manipulation
The first step will be tokenizing the list of ingredients in Ingredients column. After splitting them into tokens, we'll make a binary bag of words. Then we will create a dictionary with the tokens: ingredient_idx.

The next step is making a document-term matrix (DTM). Here each cosmetic product will correspond to a document, and each chemical composition will correspond to a term.

[image] 
