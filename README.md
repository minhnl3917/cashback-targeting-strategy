# Credit Risk Modeling & Customer Segmentation: Cashback Offer Targeting Analysis

## Project Overview

This project simulates the launch of a 5% cash-back offer and develops a data-driven targeting strategy under marketing budget constraint. The main objective is to identify which customer segments should be prioritized in order to maximize offer adoption while controlling credit risk exposure. By using behavioral metrics, customer segmentation, logistical regression modeling, and scenarios analysis, I evaluated multiple scenarios to determine the most effective customer group to balance growth and efficiency.

## Business Problem

How should a financial institution target customers for a new cash-back offer to maximize adoption and value while managing risk and limited resources?

- Which customers should be targeted?
- How does campaign outreach impact offer adoption rate?
- What is the most optimal target group to maximize growth while limiting credit risk exposure?


## Success Metrics

- Offer adoption rate
- Incremental customer engagement (proxy)
- Risk exposure (default proxy)


## Model Evaluation

The logistic regression model achieved an AUC of approximately 0.73, indicating a relatively strong ranking capability as the model can correctly rank 
an adopter higher than a non-adopter about 73% of the time.

- Key Factors
    - Higher engagement -> Increased adoption likelihood
    - Higher utilization -> Decrease adoption likelihood
    - Default history -> Decrease adoption likelihood


## Key Insights

- Targeting top 20% → 1,263 expected adopters (21.1% adoption rate)
- Targeting top 30% → 1,791 expected adopters (19.9% adoption rate)
- Targeting top 40% → 2,262 expected adopters (18.9% adoption rate)
- Zero default risk exposure across all targeting scenarios

Expanding targeting from top 20% to top 30% increased total adopters by roughly 42% while maintaining zero default exposure, despite a slight decline in adoption rate.  


## Final Recommendation

Target the top 30% of customers ranked by predicted adoption probability to meaningfully increase growth and efficiency.



## Requirements

- pandas
- numpy
- scikit-learn
- openpyxl
