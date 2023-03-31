# JPMC Task 3

**How Developed Graph:**

As in Task 2, two stocks are displayed and their pricing over time is displayed with one caveat; tracking the 12 month historical average ratio between stock ABC and DEF instead of the top\_ask\_price. In order to help determine a trading opportunity, differing upper and lower bounds are tested to demonstrate aggressive vs conservative alerting behavior via a trigger alert. We also implement a timestamp with row-pivots along the x-axis of the graph to track our ratios against time. All these attributes are added to the element under the componentDidMount method. Moreover, the Row interface must match the new schema in DataManipulator.ts Finally,  updated generateRow function of the DataManipulator class to properly process the raw server data passed to it so that it can return the processed data which will be rendered by the Graph component’s table.


**Key Insights for Traders:**

Using the generated graph of ratios, we can find when two individual stocks have a negative correlation to each other. This is very valuable when building a well-diversified portfolio as when one part of a portfolio falls in price, another may rise. This ensures losses are limited. Examples are financial stocks such as banks or insurance companies tend to get a boost when interest rates rise, while the real estate and utilities sector get hit particularly hard given an interest rate increase. The more positive a correlation, or the higher the ratio climbs  mean each stock is moving in tandem with each other.

Furthermore, this graph can give traders an understanding of how inexpensive or expensive the stock is relative to the market. It can also extend to other must-have metrics for value estimation such as P/E,  P/CF, etc after updating the schema.

Reading from the below graph (next page)generated we can see the negative correlation occurring from 4/11/21 to 7/18/21.

**Graph: (+/- .04):**

![](Aspose.Words.4fdf29d2-2aa1-490f-9250-9a20091aa910.001.png)
