# Macroeconomic Forecasting with VAR, VECM, and Threshold Models

### Forecasting GDP, Inflation, Unemployment, and Interest Rates Using Modern Time-Series Econometrics

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Econometrics](https://img.shields.io/badge/Econometrics-00599C?style=for-the-badge)
![Forecasting](https://img.shields.io/badge/Forecasting-16A085?style=for-the-badge)
![Time Series](https://img.shields.io/badge/Time%20Series-E67E22?style=for-the-badge)
![Macroeconomics](https://img.shields.io/badge/Macroeconomics-8E44AD?style=for-the-badge)

## Quick Links

[![Website](https://img.shields.io/badge/Website-cudapuca.base44.app-black?style=for-the-badge)](https://cudapuca.base44.app)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Daniel%20Puente-blue?style=for-the-badge\&logo=linkedin)](https://www.linkedin.com/in/danielpuente/)
[![Gmail](https://img.shields.io/badge/Gmail-danielpuent02%40gmail.com-D14836?style=for-the-badge\&logo=gmail\&logoColor=white)](mailto:danielpuent02@gmail.com)
[![Instagram](https://img.shields.io/badge/Running-dandrunner-E4405F?style=for-the-badge\&logo=instagram\&logoColor=white)](https://www.instagram.com/dandrunner)



---

## Why I Built This Project

I've always been fascinated by how economists try to understand the future.

Inflation, interest rates, unemployment, and economic growth are deeply connected, yet forecasting them is incredibly difficult. This project introduced me to some of the most important tools in modern time-series econometrics, including cointegration analysis, vector autoregressions, and error-correction models.

---

## Project Overview

This project analyzes Canadian macroeconomic data using advanced econometric forecasting techniques.

The analysis focuses on four key economic indicators:

- GDP
- Inflation (CPI)
- Unemployment
- Target Interest Rate

The goal was to compare multiple forecasting frameworks and evaluate which models perform best across different economic variables.

---

## Project Highlights

- Conducted Johansen Cointegration Testing
- Identified long-run equilibrium relationships among macroeconomic variables
- Implemented VAR, VECM, and TVAR models
- Performed rolling time-series cross-validation
- Compared forecasting performance using Mean Squared Error (MSE)
- Combined Python and R through the `rpy2` framework
- Forecasted GDP, Inflation, Unemployment, and Interest Rates

---

## Mathematical Framework

### Cointegration

Macroeconomic variables often move together over the long run.

The Johansen Cointegration Test was used to determine whether long-run equilibrium relationships existed among the variables.

The general relationship can be written as:

`β'Yₜ = 0`

where:

- Yₜ = vector of macroeconomic variables
- β = long-run equilibrium coefficients

The analysis identified **two cointegrating relationships**, suggesting that the variables share meaningful long-run economic connections.

---

### Vector Autoregression (VAR)

VAR models allow each variable to depend on both:

- Its own past values
- The past values of all other variables

General form:

`Yₜ = A₁Yₜ₋₁ + A₂Yₜ₋₂ + ... + εₜ`

This framework captures dynamic interactions among economic indicators.

---

### Vector Error Correction Model (VECM)

When variables are cointegrated, VECM incorporates both:

- Short-run dynamics
- Long-run equilibrium relationships

General form:

`ΔYₜ = αβ'Yₜ₋₁ + ΓΔYₜ₋₁ + εₜ`

where:

- α measures adjustment toward equilibrium
- β captures long-run relationships

---

### Threshold VAR (TVAR)

Economic relationships are not always linear.

TVAR models allow different dynamics depending on economic conditions, making them useful when behavior changes during expansions, recessions, or periods of economic stress.

---

## Data

The dataset contains Canadian macroeconomic indicators beginning in 2015, including:

- GDP
- Consumer Price Index (CPI)
- Unemployment Rate
- Target Interest Rate

To prepare the data for modeling:

- Missing values were removed
- Variables were transformed to stationary series
- First differences were computed where appropriate

---

## Methodology

### Step 1: Cointegration Testing

I first used the Johansen Trace Test to determine whether long-run equilibrium relationships existed among the variables.

The results indicated the presence of **two cointegrating relationships**, supporting the use of Vector Error Correction Models.

### Step 2: Model Estimation

Three forecasting frameworks were estimated:

- VAR
- VECM
- TVAR

Each model was evaluated under multiple lag specifications.

### Step 3: Time-Series Cross Validation

Instead of evaluating models using a simple train-test split, I implemented rolling time-series validation.

This approach better reflects real-world forecasting, where only historical information is available at each point in time.

### Step 4: Forecast Evaluation

Model performance was assessed using Mean Squared Error (MSE) across all variables.

---

## Key Findings

Different economic variables were best forecasted by different models.

### Best Performing Models

| Variable | Best Model |
|-----------|------------|
| Inflation (CPI) | VAR (Lag 2) |
| GDP | TVAR (Lag 2) |
| Unemployment | VECM (Lag 2) |
| Interest Rate | TVAR (Lag 1) |

One of the most interesting findings was that no single model consistently outperformed the others.

Different economic variables responded better to different forecasting frameworks, highlighting the complexity of macroeconomic systems and the importance of selecting models based on the problem being studied.

---

## What I Learned

This project changed how I think about forecasting.

Before working on it, I assumed the best model would consistently outperform the others. Instead, I learned that different economic variables often require different modeling approaches.

I also gained a much deeper understanding of:

- Cointegration
- Long-run equilibrium relationships
- Economic forecasting
- Multivariate time-series analysis
- Model validation

Most importantly, I learned that forecasting is not simply about generating predictions. It is about understanding the structure of economic relationships and making informed decisions under uncertainty.

---

## Skills 🥵🔥

### Econometrics

- Johansen Cointegration Testing
- VAR Models
- VECM Models
- TVAR Models
- Forecast Evaluation

### Statistics

- Time Series Analysis
- Multivariate Modeling
- Forecast Validation
- Mean Squared Error Analysis

### Data Science

- Data Cleaning
- Exploratory Analysis
- Statistical Programming
- Data Visualization

### Tools

- Python
- R
- rpy2
- Statsmodels
- tsDyn
- Pandas
- NumPy
- Matplotlib
- Git
- GitHub


---

## About Me

I'm **Daniel Puente**, a Statistics and Economics graduate from the University of Toronto and an incoming Master of Management in Analytics student at McGill University.
