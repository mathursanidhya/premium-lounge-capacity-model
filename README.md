# Premium Lounge Capacity & Nonlinear Congestion Modeling Framework

## Overview

This project develops a regime-aware forecasting and nonlinear congestion modeling framework to inform capital expansion decisions for premium airport lounges.

Among the most valued premium benefits are airport lounge access privileges. As premium card portfolios expand, lounge utilization increases accordingly. This creates a strategic challenge:
How should a credit card issuer anticipate and plan lounge capacity as premium customer penetration grows?

Unlike retail environments, lounge congestion behaves nonlinearly. Small increases in premium demand can materially amplify peak-hour crowding once seating thresholds are approached. Average-volume forecasts systematically understate peak-hour congestion risk.

---

## Core Strategic Questions

This model answers three capital-planning questions:

1. What is the stabilized 2024 passenger baseline for a premium-aligned airport terminal?
2. How does terminal passenger growth translate into peak lounge demand?
3. At what growth threshold does congestion risk justify seating expansion?

---

## Key Insight

Congestion behaves nonlinearly near saturation.

Under a +6% passenger growth scenario:
- A 130-seat configuration produces ~40% peak overflow probability.
- Maintaining ≤20% overflow probability requires approximately 145 seats.
- Offsetting a 6% demand increase requires ~11–12% seating expansion.

Capacity decisions based on average utilization systematically underestimate peak-hour risk.

---

## Methodology

The framework integrates:

• Structural time-series analysis to isolate post-COVID passenger regime stabilization  
• Hybrid seasonal projection (2023 stabilized level × pre-COVID seasonal index)  
• Demand translation funnel (terminal volume → premium eligible → peak arrivals)  
• Peak occupancy modeling using Little’s Law  
• Stochastic arrival dispersion to estimate overflow probability  
• Sensitivity analysis across growth, premium mix, dwell time, and peak compression  
• Financial optimization comparing expansion cost vs. denied-entry losses  

---

## Model Architecture

Passenger Volume Forecast  
→ Premium Eligibility Funnel  
→ Peak Arrival Concentration  
→ Occupancy = Arrival Rate × Dwell Time  
→ Probabilistic Overflow Estimation  
→ Capital Trigger Identification  

---

## Sensitivity Findings

Relative congestion drivers ranked by structural impact:

1. Premium cabin share  
2. Card penetration  
3. Peak-hour concentration  
4. Dwell time  
5. Aggregate passenger growth  

Premium mix shifts exert greater congestion leverage than equivalent passenger growth.

---

## Financial Tradeoff Analysis

The model estimates:

- Annual lost contribution from denied-entry events under constrained capacity  
- Annualized seat expansion cost (7-year life, 10% hurdle rate)  
- Net economic benefit across seating configurations  

Findings show a financial optimum near ~140 seats, while a 145-seat footprint aligns with a ≤20% overflow service benchmark.

This distinction separates pure economic optimization from strategic service-level governance.


---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- SciPy
- Jupyter Notebook

---

## Limitations

This framework is designed for strategic capital sensitivity analysis.

It does not:
- Model real-time airline departure banks
- Simulate dynamic queue management or throttling behavior
- Incorporate multi-lounge substitution effects
- Serve as a macroeconomic demand forecast

Synthetic parameters (premium share, card penetration, peak concentration) are structural stress inputs used to evaluate sensitivity dominance rather than predict precise utilization.

---

## Strategic Implication

### Capacity as a Portfolio and Retention Lever

Lounge capacity should be integrated into portfolio governance rather than treated as an isolated facilities decision. As premium penetration increases, congestion exposure becomes directly linked to customer experience consistency. 

Denied-entry events introduce variability into a benefit that underpins premium acquisition and retention economics. When access reliability deteriorates, the expected lifetime value assumptions embedded in growth strategy are weakened. 

As premium penetration increases, crowding shifts from an operational issue to a customer retention risk. Capacity planning should therefore be aligned with growth targets and evaluated proactively within product strategy cycles. 

### Recommendation 

Under the +6% growth scenario, a 130-seat configuration produces structural instability during peak months. To maintain overflow probability below 20% and preserve a consistent premium experience, planning toward a ~145-seat footprint is recommended. This adjustment is not driven by average demand expansion alone, but by the interaction between portfolio growth, peak-hour concentration, and dwell dynamics. 

The key takeaway is that premium growth interacts with peak concentration and dwell time in a nonlinear way once utilization approaches capacity. At that point, small demand increases require disproportionately larger seating expansion to maintain access reliability. Aligning portfolio growth with peak-capacity thresholds will prevent reactive capital deployment and protect retention economics.

---

## Author

Sanidhya Mathur

