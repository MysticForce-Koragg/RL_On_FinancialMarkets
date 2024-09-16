# Reinforcement Learning on StockMarket

This project focuses on developing a Reinforcement Learning (RL) agent to make trade decisions based on market data. The agent is trained using weekly and daily candle data, reducing noise and outliers. Key indicators such as RSI, ATR, VWAP, and 52-week High/Low are used as inputs, along with position data, to provide a comprehensive market view.

The agent's actions include Long, Short, and Hold, with the selected action determined by the argmax of the neural network's outputs.

Reward Function:

Initial reward: -500 points.
Closing a position with profit: +300 points.
Opening a position: 0 points (no reward).
Holding a position or not opening: -100 points.
Closing a position with a loss: -300 points.
This reward structure is designed to encourage profitable trades while penalizing indecision and losses.
