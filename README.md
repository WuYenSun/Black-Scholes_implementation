# Black-Scholes_implementation

This note provides an examination of various numerical methods employed in the implementation of vanilla options within the Black-Scholes economy. 
The methods discussed encompass the Black-Scholes closed-form formula, Monte Carlo simulation, and numerical integration. 
Furthermore, the note delves into the interpretation of N(d1) and N(d2) in the Black-Scholes formula, elucidating their significance as risk-neutral probabilities under the underlying and money market account numeraires, respectively.

# Introduction
The Black-Scholes closed-form formula stands as a baseline and pioneer in option pricing theory, offering a mathematical expression for determining the fair value of a vanilla option. 
This formula considers various parameters, such as the current price of the underlying asset, the strike price of the option, the time to expiration, the risk-free interest rate, and the volatility of the underlying asset. 
By incorporating these inputs, the formula yields a precise estimate of the option's value within the Black-Scholes economy.

In addition to the closed-form formula, the note explores the Monte Carlo simulation method, which utilizes random sampling techniques to simulate possible future paths of the underlying asset's price. 
By repeatedly simulating the asset's price movement and calculating the corresponding option values, a pricing estimate can be obtained. 
Monte Carlo simulation proves particularly useful when dealing with complex options or when closed-form solutions are not readily available.

Moreover, the note investigates numerical integration techniques as a viable approach to option pricing. 
Numerical integration methods, such as the trapezoidal rule or Simpson's rule, offer a means to approximate the integral involved in the risk-neutral pricing paradigm. 
By discretizing the integral and employing numerical techniques, a numerical solution for the option's value can be obtained with high precision.

While it is widely recognized that N(d2) represents the risk-neutral probability of the option expiring in-the-money, 
it is often overlooked that N(d1) also serves as the risk-neutral probability if we consider the underlying asset as the numeraire.
Gaining insights into the interpretation of N(d1) and N(d2) enhances one's understanding of option theory.
A numeraire is any positive non-dividend-paying asset. 
The idea of change of numeraire sits on the fact that a financial market is arbitrage-free if and only if there exists a numeraire and an associated equivalent measure under which each (traded) asset price divided by the numeraire is a martingale.
The unique arbitrage-free value bridges the measures.
