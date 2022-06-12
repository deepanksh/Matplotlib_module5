# Matplotlib_module5

Overview of the analysis
I conducted the analyses and visualization of the ride-sharing data very similar to Uber. I had two datasets: ride data with location, date and fare for every ride, and city data which describes type of city and number of drivers. The goal was to compare quantity and fares of rides in every city type: urban, suburban and rural; create clear visualization with matplotlib library and provide recommendation to the CEO for addressing any disparities among the city types.

During the analysis I’ve used Jupyter Notebook, pandas and matplotlib libraries.

Results
In order to perform the analysis, I merged datasets using left join based on the city column and got a one dataset with all available data. First of all, I created summary dataframe by city type. It has revealed first insight - there are few drivers and rides in rural cities with higher average fares compare to urban cities:

There are 13 times more rides in urban cities compare to rural cities (1,625 vs 125 rides)
The average fare per ride is 1.4 times less and average fare per driver is 3.4 times less in urban cities compare to rural cities ($24.53 vs $34.62 and $16.57 vs $55.49)
The total fares in urban cities is 9 times higher than in rural cities and 2 times higher than suburban cities. ($39,854.38 vs $4,327.93) Summary_of_rides
Then I created a multiple line plot that shows the total weekly of the fares for each type of city. The yellow line for urban cities is higher than red and blue lines for suburban and rural cities, respectively. That means ride-sharing company has more total fares and revenue in urban cities rather than in suburban and rural cities. Summary_chart

For example, the maximum total weekly fares in urban cities is close to $2500 at the end of February, while the maximum total weekly fares in rural cities is $500 at the beginning of April.

Summary
While the urban cities rides make more revenue, the rural cities rides are more profitable. So, I would focus on improving profitability of urban cities rides.

I would recommend to reduce number of drivers in urban cities. There are 2,405 drivers which made only 1,625 rides. That means not every driver has done at least one ride. Reducing number of drivers will increase average fare per driver, as now it is 3.4 times less compare to rural cities.

Additional analysis of ride duration should be done. It may be insightful to calculate average fare per 1 minute or 1 kilometer and compare the value among city types. If the fare for 1 minute of ride in rural cities is significantly higher than fare in urban cities, ride fare may be increased for urban city types. It helps to increase average fare per ride in urban cities and get even more revenue.