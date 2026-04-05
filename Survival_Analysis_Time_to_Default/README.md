##### The Portfolio Risk Profile
* Survival Modeling:  
Utilized **Kaplan-Meier estimates** to model the survival probability of a 74,000-loan portfolio.
* Critical Risk Window:  
Identified a critical risk horizon between **months 5 and 40**. During this 35-month window, the cumulative survival probability declined from nearly 100% to 75%, representing the period of peak hazard for the portfolio. Beyond month 60, while a sharp decline is observed, the widening confidence intervals and dwindling 'At-Risk' count (n < 150) suggest that risk interventions are most effective if deployed before the 40-month maturity mark.
* Proactive Intervention:  
This longitudinal analysis provides the foundation for time-dependent classifiers, enabling the bank to trigger risk interventions prior to peak default periods.  
##### Multivariate Risk Drivers (Cox Proportional Hazards)
To analyze granular risk drivers, I implemented a **Cox Proportional Hazards (CPH)** model. This allowed for the quantification of specific features on the baseline hazard of default.
* Model Performance:  
The model achieved a **Concordance Index of 0.69**, indicating strong discriminative power in ranking borrowers by their relative risk of failure ($p < 0.005$).  
* Key Risk Determinants:  
-- **Annual Income & Interest Rate:** These surfaced as the most prominent drivers of the hazard rate.  
-- **Home Ownership:** Renters demonstrated a significantly higher hazard (shorter time-to-default) compared to homeowners.

#### Strategic Conclusion:  
Borrowers characterized by low income, rental status, and high-interest loan products exhibit the highest "acceleration" toward default. This insight allows for more precise risk-based pricing and capital allocation strategies.
