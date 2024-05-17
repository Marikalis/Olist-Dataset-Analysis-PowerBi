# Data Analysis Report based on Brazilian E-Commerce Public Dataset by Olist


### Trends on e-commerce

Analysis of e-commerce data indicates a noticeable upward trend in Brazilian online shopping activity. Over a specified period, there has been a consistent increase in the volume of online purchases, suggesting a growing inclination towards e-commerce among Brazilian consumers. This trend aligns with broader global patterns indicating the increasing popularity and adoption of online shopping as a preferred retail channel

### Day of Week for Online Purchasing:

![orders_by_day_time](https://github.com/Marikalis/Olist-Dataset-Analysis-PowerBi/assets/63310952/f4ae2f18-99f3-4df6-8003-a201c6ddb6f7)

Monday and Tuesday: These days emerge as the most popular for online shopping among Brazilian customers. This could be attributed to several factors, including the start of the workweek when individuals may have more time to browse and make purchases, as well as the potential influence of promotional offers or discounts typically associated with the beginning of the week.

> **Custom Columns for Order Analysis**
> Total Orders by Weekday
> To categorize orders by weekdays, we use the DayName column. This column is populated by mapping the DayOfWeek value to its corresponding weekday name using the SWITCH function. The mapping is as follows:
> 
> ```
> DayName = SWITCH([DayOfWeek], 
>     1, "Monday",
>     2, "Tuesday",
>     3, "Wednesday",
>     4, "Thursday",
>     5, "Friday",
>     6, "Saturday",
>     7, "Sunday"
> )
> ```
> Total Orders by Time of Day
> Similarly, to classify orders by the time of day they were placed, we use the SortOrder column. This categorization helps in understanding customer preferences throughout the day. The SortOrder value is determined using the following SWITCH function:
> 
> ```
> SortOrder = SWITCH([TimeOfDay],
>     1, "Morning",
>     2, "Afternoon",
>     3, "Evening",
>     4, "Night"
> )
> ```

### Time of Day for Online Purchasing:

Afternoon: The afternoon is the preferred time for online shopping among Brazilian customers. This timeframe typically spans from early afternoon to early evening. This preference may be influenced by factors such as convenience, availability of leisure time, and access to digital devices during breaks from work or other activities.

### Insights:

![order_status_over_time](https://github.com/Marikalis/Olist-Dataset-Analysis-PowerBi/assets/63310952/2b73dabf-f0b0-41e0-9576-38a08321d16b)

*	Consumer Behavior: The growing trend in Brazilian e-commerce suggests a shift in consumer behavior towards online shopping, driven by factors such as convenience, accessibility, and an increasing digital presence of retailers.
*	Strategic Considerations: Retailers can leverage insights into the preferred days and times for online shopping to optimize marketing strategies, schedule promotional campaigns, and enhance customer engagement.
*	Infrastructure and Support: To accommodate the increasing demand for online shopping, retailers should ensure robust infrastructure, including reliable website performance, secure payment gateways, and efficient logistics and delivery services.
*	Personalized Marketing: Tailoring marketing efforts and promotional offers to align with peak shopping times and consumer preferences can help retailers maximize sales and improve customer satisfaction.

## Conclusion:
The analysis indicates a growing trend in Brazilian e-commerce, with Monday and Tuesday emerging as the most popular days for online shopping, particularly during the afternoon. By understanding and capitalizing on these trends, retailers can effectively engage with Brazilian consumers, drive sales, and capitalize on the expanding opportunities in the e-commerce landscape.

![orders_over_time](https://github.com/Marikalis/Olist-Dataset-Analysis-PowerBi/assets/63310952/d188ffb7-282b-4424-8c57-f20d02950637)

