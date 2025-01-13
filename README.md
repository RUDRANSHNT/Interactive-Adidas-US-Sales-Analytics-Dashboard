# Interactive Adidas US Sales Analytics Dashboard

![Adidas Dashboard Screenshot](https://github.com/user-attachments/assets/ab27d8c4-1b83-41c8-8bbe-df04ea012b55)

**Table of Contents**

1. Project Discription
2. Key challenges addressed by the dashboard
3. Steps Followed
4. Insights and analysis
5. Dataset Information
6. Note

**Project Description**

The objective of the Interactive Adidas US Sales Analytics Dashboard is to provide a comprehensive and interactive solution for tracking and analyzing key performance indicators (KPIs) related to Adidas' sales and operations in the United States. The dashboard aims to give business users, analysts, and decision-makers a clear and dynamic view of performance across multiple dimensions, enabling them to make data-driven decisions to improve operational efficiency and drive sales growth.

**Key challenges addressed by the dashboard:**

1. **Comprehensive Data Visualization**: Consolidating key performance metrics (KPIs) like Total Sales, Total Operating Expenses, profit, and Total Units sold into a unified, interactive view, addressing limitations of traditional static reports.

2. **Interactive Drill-down**: Enabling users to explore data at various levels (region, state, city, time) for a deeper insights into performance.

3. **Multi-KPI Performance Analysis**: Presenting financial and operational KPIs together to easily identify trends and anomalies.

4. **Sales Channel Insights**: Showing sales distribution by method (in-store, outlet, online) to understand channel contributions.

5. **Time-Based Trends**: Analyzing performance over time through time series and quarterly breakdowns for better forecasting and decision-making.


By providing an easy-to-navigate and interactive dashboard, the solution ensures that users can efficiently explore Adidas’ sales data and uncover actionable insights to drive strategic business decisions.

**Steps Followed:**

1. Imported the Adidas Sales dataset into **Power BI desktop**, as an XLSX excel file.

2. Transformed the dataset in **Power Query** by removing unnecessary rows, changing the first row as headers, performing appropriate data type conversion of relevant columns, and creating a new column named 'Operational Expenses' using the following **DAX** expression:

       Operating Expenses = Data[Total Sales] - Data[Operating  Profit]

3. Defined the relevant Key Performance Indicators (KPIs) as card graphics on the top of the dashboard highlighting Total Sales, Total Operating Expenses, Total Operating Profit, Average Operating Margin and Total Units Sold.

4. Utilized the stacked bar chart to visualize the breakdown of total units sold by each of the 5 US regions, namely the West, Northeast, South, Southeast and the Midwest. The user can drill down by state and city for each region using the drill-down functionality.

5. Created a treemap visualization to represent the distribution of Total Sales by each retailer, namely West Gear, Footlocker, Sports Direct, Kohl's, Amazon and Walmart.

6. Employed the clustered column chart to visualize the breakdown of total sales, total operating expenses and total operating profit by each region. The user can drill down these KPIs for each region by state and city-wise breakdown using the drill down functionality.

7. Harnessed the line and clustered column chart to visualize the time series analysis of the sales performance. The clustered column part contained total sales, total operating expenses, and total operating profit for different quarters. The time analysis can also be drilled down by month and day using the drill down function, for a more thorough analysis. The line part represented the trend of total units sold by each quarter.

8. Created a table to represent the sales performance by product. The sales column contained data bars for a more visual representation of the sales performance. Finally, a donut chart was created to visualized the contribution of each sales channel, namely in-store, outlet and online, towards the total sales figure.

The interactive functionality of the Adidas US Sales Analytics Dashboard allows users to drill down by region, state, or city, apply filters (e.g., time period, sales method), and analyze time-based trends. Dynamic KPIs update based on user selections, enabling tailored, real-time data exploration for informed decision-making. 

**Insights and Analysis:**

The following inferences can be drawn from the dashboard:

    Total Sales: $899.90 M

    Total Operating Expenses: $567.77 M

    Total Operating Profit: $332.13 M

    Average Operating Margin: 42.3%

    Total Units Sold: 2.48 M

Western united states has the highest demand for adidas products (687k units sold) with Northeast (501k units) and southern (492k units) regions having an almost equal demand. The midwest (391k units) has the lowest demand for adidas products.

![111](https://github.com/user-attachments/assets/164b2de3-b10e-496b-84ab-03bd3e946a9d)


Retailers like West Gear ($242.96 M in sales) and footlocker ($220.09 M in sales) have the highest sales where e-commerce giants like Walmart ($74.56 M in sales) and Amazon ($77.70M in sales) are the bottom-most performing retailers. Sports direct has the highest operating margin (44.49%) while for others, its almost around 41%.

![treemap](https://github.com/user-attachments/assets/4bcf663f-d92a-4b8a-8188-a6c214409032)



Although the west drives the highest sales ($270 M), its operating expenses are also high ($180 M), thus leading to a not so high operating profit ($90 M). In fact, South has the highest average operating margin (46.69%) while west has the lowest (39.67%). This can be due to a lower cost of living, low minimum wages in the southern region along with other factors.

![1234](https://github.com/user-attachments/assets/214a07aa-d375-4dea-805f-6676327eae5d)


The sales peak around mid summer (june, july). This can be understood in the following manner; summers lead to an increase in outdoor activites leading to an increase in sportswear demand. Moreover, multiple national and local level sporting events (like NFL, NBA etc) are organized during summers which also drive merchandise and sportswear demand.

![time series](https://github.com/user-attachments/assets/ed8854bb-c487-4a65-a072-1e7c27238219)


Men's street footwear ($208.82 M in sales) and women's apparel ($179.03 M in sales) are the top performing products. Adidas has successfully collaborated with celebrities (like Kanye West for Yeezy) and designers, boosting the visibility and desirability of its footwear. The athleisure trend, which blends athletic and leisure wear, has been a major driver in women's apparel. Adidas has successfully capitalized on this by offering fashionable, functional activewear that fits into everyday casual styles.

![table](https://github.com/user-attachments/assets/b3a58114-e990-4fe9-9fea-d920d616374d)


Adidas has traditionally been focused on footwear. Nike has been a dominant player in the women’s athletic footwear market, particularly with its innovative designs, technology, and heavy investment in influencer marketing. For women’s athletic footwear, the increasing demand for fashionable, lifestyle sneakers has shifted focus away from performance-focused shoes, which is evident from the above performance data.

In-store sales channel drives the most sales ($357 M) while outlet ($296 M) and online ($248 M) methods are also different in performance. However, online method drives the highest operating margins (46.42%), whereas in-store has the lowest average operating margin (35.61%).

![donut chart](https://github.com/user-attachments/assets/224a1408-c5a6-4ad0-9d01-9385950dd415)


Northeast consumers prefer an in-store experience. West Gear and Kohl's have west as their consumer base while Amazon has northeast, Footlocker has the east coast, Walmart and Sports direct have southern states as their consumer base for Adidas products.

![northeast](https://github.com/user-attachments/assets/aedee236-a674-4870-ab3c-6fbd9fde63af)

**Dataset Information:**
The Adidas sales dataset contains the following columns:

    Retailer
    Retailer ID
    Invoice Date
    Region
    State
    City
    Product
    Price Per Unit
    Units Sold
    Total Sales
    Operating Profit
    Operating Margin
    Sales Method

**Note:**
The above insights are inferred on a national scale. These insights may differ once we drill down specifically by product, region, and/or retailer.
