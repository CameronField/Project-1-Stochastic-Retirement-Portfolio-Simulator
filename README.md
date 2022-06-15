# Project 1: Stochastic Retirement Portfolio Simulator

### General Discription
Retirement portfolio simulator that incorporates probabilistic market returns

## Intro

The goal of this project is to present a dynamic, probabilistic, and helpful visualization of an investor's retirement portfolio across his or her lifespan.

Alternativevly, his project can be used by any investor who wants to stress-test their retirement portfolio and quantify the likelihood that their strategy will not run out of money. When designing this project, I tried to take into account all the major variables that an investor should consider when planning their retirement.

Instead of presenting a simple portfolio calculator that uses fixed return rates each year, the goal was to use the inverse-normal function to generate sudo-random returns rates that mimic the actual behavior of the market (historically, market returns are normally distributed). Given the amount of parameters used in this project, I honestly had no idea where to start with an analytical solution, so I chose to use the monte-carlo method to derive insights.

The model is entirely dymanic, so feel free to change the parameters to your liking, but in its current form, its defaults are set to numbers that match the average american retirement investor.

Please note that in its current form, this does not take into consideration tax-advantaged retirement accounts like Roth 401(k), Roth TSP, HRA, or employer contributions.

## Diversified Investing Strategy
One motivator for this project was that I kept getting burned doing active trading strategies and I started looking for a new strategy. At least for me, active investing is not tax efficient, it's time-consuming, and even in a good year, I tended to not outperform the market. So after a bit of research, I've come to the conclusion that the best strategy is just to invest in the market itself and buy an index fund (see Buffet et al).

Diversification is the most effective strategy against isolated portfolio risks. As noted in the Markowitz model first published in 1952, given a group of assets, the most efficient portfolios of those assets are the combinations that result in the highest returns with the lowest risk, with standard-deviation being a proxy for risk. The more uncorrelated assets you have in that basket of assets, the more diversified you become, and the better your expected returns become. These optimal combinations, otherwise known as the 'efficient-frontier' are the foundation of modern-portfolio theory, and hence, this project.

## Jupyter Notebook Version vs Excel Version
I initially created this project on Excel, but due to the long calculation times, I decided to try it out on Python in order to add more functionality and speed. Both the jupyter notebook and excel versions are included in this repository
