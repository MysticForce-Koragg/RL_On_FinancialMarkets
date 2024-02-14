# Reinforcement Learning on StockMarket

This project aim to make trade decisions using RL Agent.

Weekly and daily candle data is used to train the agent to avoid noise and outliers. Most popular indicators and price levels such as RSI, ATR, VWAP, 52-week High/Low and etc is used as observations along with position data.

The actions for the agents are Long, Short, and Do Nothing. The action for the observation is the argmax of the NN outputs.

Reward Fuction: Intial rewards for the agent is -500. 300 points for the closing the position with profit and No reward for opening position and -100 will be for holding the position or not opening position, for closing the position with the loss will be -300 points.
