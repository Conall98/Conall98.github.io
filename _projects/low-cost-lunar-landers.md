---
title: "How Cheaply Can Cargo Be Delivered to the Moon?"
tag: "Journal Paper"
order: 1
description: "A probabilistic cost-and-mass study of ten lunar mission architectures, asking how low the per-kilogram cost of delivering cargo to the lunar surface can realistically be pushed, and what it would take to get there."
image: ""
---


## The question

Lunar exploration is in a renaissance. Between 1976 and 2013 no lander touched the surface; since then sixteen have been launched, with at least a dozen more planned by 2031. Both China and the United States are planning permanently crewed bases at the lunar south pole. This increase in activity is what motivated this investigation into current payload delivery costs and how low those costs can plausibly fall in the future.

## How we answered it

By building a probabilistic cost-and-mass estimation tool called **P-CARAMEL** (Probabilistic Cost Approximation by Regression-based Algorithm for Mass Estimation of Landers). Instead of producing single-point estimates, it runs Monte Carlo simulations using:

- new statistical sizing rules derived from a fresh database of 33 lunar landers (Luna 9 through Hakuto-R M2) and a subsystem-level database of 34 designs;
- industry-standard parametric cost relationships from TrueCost and the QuickCost model;
- a launcher database that selects the cheapest viable rocket for each mission, On both rideshare and dedicated launch basis.

By defining five alternative mission architectures (MA) — expendable single-launch landers like Blue Ghost and IM-1, reusable architectures with one or two refuellable space-tugs, electric-propulsion tugs, and weak-stability-boundary trajectories like Hakuto R — and performed a payload mass and #mission run sweep to capture the cost behaviour with increasing.

## What we found

Recent commercial CLPS missions cost between **$1.3M and $5.7M/kg**. This is an improvement on the Apollo delivered cargo cost of roughly **$8.5M/kg** in 2020 dollars.

The cheapest architecture in the study, **MA5** (a single expendable lander on a weak-stability-boundary trajectory), came out at a median of **€213,000/kg**, with a 5th-percentile estimate of **€125,000/kg**.


Three things drive the reduction:

1. **Spread development cost over many missions.** Most current cost-per-kg is fixed cost amortised over one or two flights. Run the same architecture five, ten, twenty times and the per-kg cost falls sharply.
2. **Make payloads bigger.** Today's landers carry 30–800 kg. Pushing payload up to 2,000 kg or more cuts per-kg cost dramatically, because most of the lander's mass is propellant and structure that doesn't grow as quickly as payload.
3. **Stay expendable, for now.** This was the most counter-intuitive result. Reusable architectures (MA2, MA3, MA4) carry a "jeep problem" penalty — the propellant they need for the return trip has to be lifted from Earth too, and propellant required to lift that extra propellant compounds. Until propellant production on the lunar surface is possible, reusable lunar landers will stay more expensive per kilogram than expendable ones no matter how many re-uses there are.

The one exception is **MA4**, which uses an electrically-propelled space tug. Its very high specific impulse means it escapes most of the jeep problem and approaches the expendable cost line. It's slow, but it's cheap.

## Why it matters

This paper shows what is possible without exotic new technology — just by running the same well-understood architectures more often, building landers in series, and scaling up payload sizes, the cost can be reduced by around 80%.
## The full paper

[Low-Cost Uncrewed Lunar Landers: How Cheaply Can Cargo Be Delivered to the Moon?](https://www.researchgate.net/publication/405024172_Low_Cost_Lunar_Landers_How_Cheaply_Can_Cargo_Be_Delivered_to_the_Moon) — ResearchGate.

Source code for P-CARAMEL and the lander database is on GitHub: [Conall98/LLJP_ULTIMA](https://github.com/Conall98/LLJP_ULTIMA).
