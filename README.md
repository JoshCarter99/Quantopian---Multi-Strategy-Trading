# Quantopian---Multi-Strategy-Trading
Quantopian project that switches between multiple strategies based on current indicators like VaR. 


## Inspiration

We realised that it was quite hard to run two strategies in parallel or swap between on Quantopian, so decided to build an expanse framework for how this would be done. 

## What it does

The project simply runs one strategy, in this case just moving average crossover strategies with different portfolios, until the strategies return drops below 2 s.ds from expected. At this point this strategy stops and the other starts running.


## Why it's good.

- Using multiple strategies makes your investing more robust, so if one strategy starts to fail (e.g from changing market conditions), you can quickly swap it out for another. 

- This idea is very general (has a large breadth), and has obvious potential for expansion.

- The idea would be useful in the real world, as it builds on top of strategies that we know already work in the real world.

- We have considered the price of swapping between strategies, and so have made it so the program can only change strategies at most once a day.

- The alpha gen relies of the project relies on the alpha gen of the strategies used, so just increases the alpha gen of already used strategies

## What's next for Multi Strategy Trading

This project has a lot of potential. The next steps would include building it with more advanced strategies; a better way to evaluate how a strategy is performing; more strategies to swap between; and to allow for a weighting between each strategy, rather than just stopping one and starting another. 

