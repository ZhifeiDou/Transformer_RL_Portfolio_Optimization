# Leveraging Transformer in Deep Reinforcement Learning for Portfolio Optimization
This is the course project for MIE1666 2024 Fall Team 5: 
**Leveraging Transformer in Deep Reinforcement Learning for Portfolio Optimization.**

**Categories:** [Deep Reinforcement Learning, Quadratic Programming Optimization, Portfolio Optimization]

**Keywords:** [Transformer, LSTM, Proximal Policy Optimization (PPO), Quadratic Programming (QP), Differential Sharpe Ratio]

**Project Abstract:** This project explores the use of Transformer models within a Deep Reinforcement Learning
(DRL) framework for portfolio optimization. Inspired by the paper ‘Deep Reinforcement
Learning for Optimal Portfolio Allocation’, by the JP Morgan AI Research Group, as financial
markets grow increasingly complex, traditional methods, such as Mean-Variance Optimization
(MVO), often struggle to adapt to dynamic market conditions. Also inspired by breakthroughs in
deep learning and the transformative "Attention Is All You Need" paper, this work aims to
leverage the unique capabilities of Transformers to enhance decision-making in portfolio
management. The team hypothesized that Transformers can better capture the intricate temporal
dependencies inherent in financial data. To test this hypothesis, the team employed a
Transformer-based Actor-Critic model to simulate financial environments using real-world data
from five prominent Chinese stocks. The approach is benchmarked against three baseline
models: a quadratic programming-based optimizer, fully connected neural networks (ANN), and
Long Short-Term Memory Networks (LSTM). The comparison is conducted to evaluate whether
Transformers can outperform these established approaches in balancing risk and return while
managing portfolio allocations in a dynamic financial context. The results indicate that while the
Transformer-based DRL model is competitive, it does not significantly outperform the baseline
models. This is likely due to limitations such as the simplified environment and the use of
daily-level data, which restrict the model's ability to capture more intricate patterns within the
financial dataset. The findings suggest that access to more detailed minute-level data and the
incorporation of broader contextual features could further enhance the model's performance.
This research contributes to advancing portfolio optimization by integrating Transformers with
DRL, highlighting the adaptability of Transformers beyond Natural Language Processing (NLP)
applications, and offering insights into the application of advanced AI techniques in financial
decision-making.

## Full Report
The full report is available in [here](/MIE1666_Report.pdf)

## Folder and explanations:

**ft_val** -> final hyperparameter tuning for the transformer model in the deep reinforcement learning structure 

**final_comparsion** -> Train the transformer with the tuned hyperparameter setting and evaluate it with the test dataset, compare with baseline methods (Fully connected, LSTM, and QP)

**future_work** -> Effort of trying to implement 'future work' mentioned in the slide and report

## Environment required:
python 3.9/3.10
pytorch == 2.5.1
cuda == 11.8
tushare == 1.4.6
ray == 2.39.0
gymnasium == 1.0.0
numpy == 2.1.3
pandas == 2.2.3

