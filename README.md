# project_2_Group_4
lex bot stock advice

Summary: Provide stock market advice based on a person's personal type. Data was used to narrow down 4 specific personality types and each personailty type is recommended a stock based on volatility

This repository contains scripts for two deep learning recurrent neural network models. The first is a LSTM RNN model to predict stock prices for 10 tech stocks using historical closing price data. The stocks were sorted into three groups based on volatility. The second model was to clean and organize data based on personailty type.

The first model has the following architecture:

-5-day window size;

-20% dropout fraction;

-3 hidden layers;

-20 epochs; and

-batch size of 5.

-The above parameters were tuned based on model fitting.

The following question was answered based on the model:

1. Which Stock would you recommend based on the highest volatility?

Based on predicted returns, someone with high risk tolerance should buy FSR now and sell tomorrow.

![image](https://user-images.githubusercontent.com/91438431/151613987-77b1aa8d-f382-4f3b-acf2-91ef49a271da.png)

The 10 stocks were broken into 3 sectors based on volatility (high, mid, low)

High List: TSLA, NVDA, FSR

Mid List: FB, INTC, TWTR

Low List: MSFT, GOOGL, AAPL, AMZN

A for loop was created to run the LSTM for each list providing the stock recommendation for each

The second was used to clean data based on responses to personailty related questions

Participants were categorized into 4 personality types

1. Extroversion

2. Agreeableness

3. Conscientiousness

4. Openness

A bar chart was used to show participants answers to personality questions for each personality type

![image](https://user-images.githubusercontent.com/91438431/151618075-90331728-8746-411f-bbd1-50b535f5b776.png)
![image](https://user-images.githubusercontent.com/91438431/151618116-844a9800-fd75-46d6-a8d1-728e8d7f500c.png)

Used Yellowbrick API to visualize K-Elbow to find the appropriate number of clusters

Created cluster predictive model
![image](https://user-images.githubusercontent.com/91438431/151618287-3cf4f207-dea2-40d4-85ea-0f98db5b0d6a.png)

Principal Component Analysis (PCA) was used to reduce the number of variables of a data set, while preserving as much information as possible.

![image](https://user-images.githubusercontent.com/91438431/151618551-2d3c2fa8-3597-4e90-9621-096957d81846.png)

