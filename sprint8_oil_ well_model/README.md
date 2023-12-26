## Project description

We worked with OilyGiant Petroleum company on this Project. My task is to find the best region for a new well.
This project involves Machine Learning with the Business domain.

Steps to choose the location:
- Collect the oil well parameters in the selected region: oil quality and volume of reserves;
- Build a model for predicting the volume of reserves in the new wells;
- Pick the oil wells with the highest estimated values;
- Pick the region with the highest total profit for the selected oil wells.

We have data on oil samples from three regions. Parameters of each oil well in the region are already known. We want to build a model that will help to pick the region with the highest profit margin. Analyze potential profit and risks using the bootstrapping technique.


## Description of the data

- `geo_data_0.csv` - download dataset data_0
- `geo_data_1.csv` - download dataset data_1
- `geo_data_2.csv` - download dataset data_2
- `id` — unique oil well identifier
- `f0`, `f1`, `f2` — three features of points (their specific meaning is unimportant, but the features themselves are significant)
- `product` — volume of reserves in the oil well (thousand barrels).


# **Project Insight**


Through careful observation, I derived several key insights:

1. A well must contain a volume of oil exceeding 111 thousand barrels to render its investment financially viable.
2. On average, 20 million of the total 100 million data points across the three regions meet the criteria for potential development.
3. If the foremost 200 wells in each region are developed, the maximum profit, totaling nearly 40 million USD, will be achieved in Region 1.
4. Investing in the top 200 wells across the three regions will ensure profitability to each.
5. Region 0 is distinguished by the highest profitability.
6. Moreover, Region 0 exhibits the most significant number of points surpassing the threshold of 111.

Following a comprehensive analysis and the creation of the predictive model, a summary of the project is as follows:

The outcome of this project is a predictive model capable of assessing the volume of oil reserves within a well, fostering the optimism that the capital deployed will reap financial benefits. According to the predictions drawn from the model, Region 2 hosts the most abundant average oil reserves. To turn a profit, an oil well must contain at least 111 thousand barrels of oil reserves.



