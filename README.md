# Bitcoin-Bear-Put-Spread-Payoff
In this notebook, we will build the payoff graph for long 16700 strike put and short 16300 strike put on Bitcoin. A bear put spread strategy is built by going long on put option with strike price X2 and simultaneously selling a put option with a lower strike price X1. Options with same underlying and maturity. The aim of this strategy is to benefit from small negative movements in the underlying asset. It limits the upside potential as well as the downside risk.

### 1. Import libraries
First, we will import the necessary libraries.

### 2. Put payoff
We define a function that calculates the payoff from buying a put option. The function takes St which is a range of possible values of Bitcoin price at expiration, the strike price of the put option and premium of the put option as input. It returns the put option payoff.

### 3. Define parameters
We define various parameters required to calculate the put payoff. One of the parameters is the range of Bitcoin price at expiry. To calculate the Bitcoin price range at the put's expiration, we define a range for the Bitcoin price at expiry from -10% to +5% from the spot price. That is from 90% or 0.90 to 105% or 1.05 from the spot price. These range values are for illustration purposes and can be changed.

### 4. Long 16700 strike put payoff
We plot the payoff of the long 16700 strike put option.

### 5. Short 16300 strike put payoff
We plot the payoff of the short 16300 strike put option.

### 6. Bear put spread payoff
The max profit is capped at USD 305 and the max loss is limited to USD 95. Therefore, this strategy is suitable when your outlook is moderately bearish on the underlying asset.
