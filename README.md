# Wage Convergence in the Heckscher-Ohlin Model: Evidence from Puerto Rico
Research submitted to the Midwest Economics Association undergraduate research competition.

## License
The research paper is licensed under the [Creative Commons Attribution 4.0 International License (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).  
You are free to share and adapt the work, provided proper attribution is given.  
The full license text is available in the [`LICENSE2`](LICENSE2) file.

## License for Code
The code in this repository is licensed under the [MIT License](LICENSE). You are free to use, modify, and distribute the code with proper attribution.

## Introduction
ABSTRACT. This paper aims to empirically confirm the wage convergence conjecture within neoclassical economics’ Hecksher-Ohlin model in the Puerto Rican manufacturing industry over the period 1950-1987. Using time series econometrics, I isolate the effects of increased trade liberalization on Puerto Rican manufacturing wages. Log-first-differencing technique is applied due to nonstationarity in the data. Results indicate that wage convergence is observed, but shows little correlation with movements in U.S. gross national product after differencing. These results indicate that wage convergence is observed but not due to increased trade liberalization or shock effects, and highlights the limitations of real-world applications of neoclassical economic theory.

## Methodology
Used ordinary least squares (OLS) estimates with Newey-West heteroskedasticity-autocorrelation (HAC) standard errors to account for heavy autocorrelation in the series of interest. Dealing with two nonstationary time series processes, the following tests and remedies were applied to ensure our asymptotic uncorrelation and covariance stationary (second-order weak stationarity) assumptions which underlie the LLN and CLT in time-series causal analysis hold:

1. AR(1)/Breush-Godfrey AR(q) test for serial correlation (rejected), 
2. ACF/PACF of both series (highly persistent, 8+ lags show autocorrelation), 
3. Ljung-Box tests (reject at all lags), 
4. Dickey-Fuller + Koyck geometric distributed lag-form augmented Dickey-Fuller for unit root behavior (rejected), 
5. Augmented Dickey-Fuller on cointegration difference term + Engle-Granger test for cointegration (failed to reject). 

## Conclusion from tests
Two I(1) series spawning a spurious colinear relationship. Remedy: Apply differencing and Prais-Winsten/Chochrane-Orcutt FGLS if estimates hold, then HAC errors to account for heteroskedasticity/autocorrelation.
