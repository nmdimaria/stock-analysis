# stock-analysis

## Overview of Project

The goal of this analysis was to break down data on returns for 12 different stocks.

The initial code, while effective, was not as efficient as it could be. Therefore, we now refactored the code to cut out redundancies and make it more useful for larger blocks of stock data.

## Results

The refactored code shaved off a considerable amount of time (about 80% faster) for both 2017 and 2018 data sets (2017 is pictured). 

### Original Code
![Before picture](Resources/Original_Code_Runtime_ScreenShot.png)

### Refactored Code
![After picture](Resources/Refactored_Code_Runtime_Screenshot.png)



## Summary
### What are the advantages or disadvantages of refactoring code?

The main goal of refactoring code seems to be to make the code as efficient as possible; remove redundancies, unnecessary code or change a process to ignore useless data. It's a similar process to editing a book or essay. The main bulk of the content is good but it just needs to zing a little more. 

I can imagine having efficient code is important particularly when working with large data sets. Having a quick result can be the difference between someone using your work/product over someone else's. Reworking and revising code is another big part of learning how to be the best programmer you can be. Like editing that book, you see things that you would ordinarily miss in the midst of writing your code.

However, like editing, I can also see going down a bit of a rabbit hole with this process. One of my challenges with this project was that I initially tried to change way too much about the starting code. Trying to be creative and "think outside the box" can be a double edged sword (particularly when you're like me and don't know anything about programming). You can easily get lost or mess up something that was working just fine when you slice-and-dice too much.

### How do these pros and cons apply to refactoring the original VBA script?

This code ran more efficiently by assigning indexes to each stock ticker then applying that index to indexes/arrays for volumes and prices.
`
Dim tickers(12) As String

Dim tickerVolumes(12) As Long
Dim tickerStartingPrices(12) As Single
Dim tickerEndingPrices(12) As Single
`
This enabled the program to only pay attention to the rows and information that mattered instead of having to loop through every row of the spreadsheet for every peice of data.
