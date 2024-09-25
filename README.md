# Coin Flipping Simulation Analysis

This project simulates flipping 1,000 fair coins 10 times each to study the behavior of the fraction of heads obtained. The experiment focuses on analyzing three specific coins across multiple runs and comparing their behavior against the Hoeffding bound.

## Experiment Overview
The simulation involves the following steps:
1. **Flipping Coins:** 1,000 fair coins are flipped independently 10 times.
2. **Selecting Coins:**
   - `c1`: The first coin flipped.
   - `crand`: A randomly chosen coin.
   - `cmin`: The coin with the minimum frequency of heads (the earlier one in case of a tie).
3. **Calculating Fractions:** For each of the three coins, calculate the fraction of heads obtained (`ν1`, `νrand`, and `νmin`).

## Objectives
- Simulate this experiment 100,000 times to obtain distributions of `ν1`, `νrand`, and `νmin`.
- Plot histograms of these distributions.
- Estimate the probability `P[|ν − μ| > ε]` as a function of `ε` and compare it with the Hoeffding bound `2e^(-2ε²N)`.

## Results
- Visualizations include histograms for the distributions of `ν1`, `νrand`, and `νmin`.
- A graph comparing the empirical estimates with the Hoeffding bound for different values of `ε`.

## Dependencies
- Python 3.x
- Jupyter Notebook
- Required Python libraries: `numpy`, `matplotlib`, `seaborn`

## How to Run
1. Clone the repository:
   `git clone https://github.com/aliz-f/Coin-Flipping-Simulation-Analysis.git`
2. Install the required libraries:
   `pip install numpy matplotlib seaborn`
3. Open the Jupyter Notebook
