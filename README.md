# Option-Pricing-Models

This repository contains Python code demonstrating the Monte Carlo simulation method for option pricing along with Black-Scholes Pricing Model. It includes additional examples and graphs to visualize the impact of different option parameters on the simulated stock price paths. This Python project also implements the Black-Scholes option pricing formula, which calculates the theoretical price of European-style call and put options.

## Introduction

The Monte Carlo simulation is a popular numerical method for valuing financial derivatives, especially options. It involves generating a large number of random paths for the underlying asset's price and calculating the option's expected payoff based on these paths. The Black-Scholes formula is used to model the evolution of the underlying asset's price, and the Monte Carlo estimator is employed to approximate the option's price.

 The formula takes into account various factors such as the risk-free interest rate, underlying asset price, strike price, time to expiration, and volatility of the underlying asset's returns.


## Getting Started

1. Clone the repository to your local machine.

2. Make sure you have Python installed (Python 3.11 recommended).

3. Install the required libraries by running the following command:

```
pip install numpy matplotlib scipy
```

## Implementation

The Jupyter Notebook `Monte_Carlo.ipynb` contains the implementation of the Monte Carlo simulation for European call options using the Black-Scholes formula. The code includes detailed comments explaining each step of the simulation.

### Sections:

1. **Import Libraries**: Import the required libraries for mathematical operations, random number generation, and plotting.

2. **Set Random Seed**: Set a random seed to ensure reproducibility of the results.

3. **Option Parameters**: Define the parameters required for the option valuation, such as initial stock price (`S0`), strike price (`K`), time to expiration (`T`), risk-free rate (`r`), and volatility (`sigma`).

4. **Discretization Parameters**: Specify the number of time steps (`M`) and the time step size (`dt`) for discretizing the time interval.

5. **Monte Carlo Simulation**: Simulate the paths of the underlying asset using the Black-Scholes formula and the log version of the equation. The simulation is performed using NumPy's vectorized operations to speed up computation.

6. **Monte Carlo Estimator**: Calculate the option price using the Monte Carlo estimator. The estimator involves calculating the maximum of difference between the final stock price and the strike price and then taking the average over all paths.

7. **Results Output**: Display the estimated European call option price and the time taken for the Monte Carlo simulation. It also plots the first 10 simulated stock price paths.

8. **Additional Examples**: The script includes examples to modify option parameters (volatility, strike price, and time to expiration) and re-run the simulation to observe their impact on the option price. The code calculates and displays the new option prices along with graphs for the first 10 simulated stock price paths for each scenario.

## Running the Code

To run the main script, execute the following command in the terminal:

```
Black_Scholes.ipynb

Monte_Carlo.ipynb
```


The notebooks contain the Monte Carlo simulation and Black-Scholes Prediction for the original option parameters and display the estimated European call option price along with the stock price paths graph. It will then execute the additional examples, showing the impact of modified parameters on the option price and plotting the corresponding simulated stock price paths.

## Conclusion

This repository demonstrates the implementation of the Monte Carlo simulation and Black-Scholes Prediction for option pricing. The code includes additional examples with graphs to visualize how changes in option parameters affect option prices and underlying asset price paths. The Monte Carlo method provides a flexible and powerful approach to value financial derivatives, making it an essential tool for risk management and option pricing in the financial industry.
