# NLP-trading-GR5067

This project implements **sentiment-based trading strategies** using financial news headlines from 2017–2019.  
It is based on the methodology described in our paper:  
*Yufei Jing, Xinyi Zhu, Yuefei Chen (2022). Natural Language Processing in Trading.*

We develop two strategies:

1. **Baseline Sentiment Model (Strategy 1)**  
   - Generate sentiment signals from news headlines using VADER  
   - Aggregate signals into 14-day sentiment windows  
   - Compute 5-day forward stock returns  
   - Construct a **market-neutral long/short portfolio**  
   - Backtest portfolio performance  

2. **Enhanced Deep Learning Model (Strategy 2)**  
   - Use the sentiment sequence as time-series input  
   - Train **LSTM models** (2017–2018) to predict 5-day returns  
   - Test on 2019 data  
   - Build a market-neutral portfolio based on predictions  
   - Compare performance with baseline model  
