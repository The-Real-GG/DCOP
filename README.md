# Duck Curve Optimization Project
# Independent Study Project Proposal

## Title

**Modeling Grid Stability Using Computational Mathematics: Battery Optimization for Mitigating the Solar Duck Curve**

## Goal

The goal of this independent study is to investigate how computational mathematics can be used to improve electrical grid stability during periods of rapid changes in renewable energy production. Specifically, this project will develop and analyze a mathematical simulation that models the "Duck Curve" phenomenon and determines the minimum battery storage capacity required to smooth rapid increases in net electrical load during the evening hours. By combining numerical methods, optimization, and simulation, this project aims to demonstrate how computational mathematics can be applied to a real-world infrastructure problem related to disaster resilience and energy reliability.

## Research Question

**How can numerical differentiation, numerical integration, and optimization be used to determine the minimum battery storage capacity required to keep the electrical grid within a safe operating ramp rate during periods of rapid changes in solar generation?**

## Background

As renewable energy becomes a larger portion of the electrical grid, solar generation creates a well-known challenge known as the *Duck Curve*. During the day, abundant solar production reduces the amount of power supplied by conventional generators. At sunset, however, solar production rapidly decreases while electricity demand simultaneously increases as people return home. This creates a steep increase in net load that conventional generators may struggle to follow quickly enough, increasing the risk of grid instability or controlled power outages during extreme weather events.

Rather than viewing batteries solely as energy storage devices, this project investigates their role as dynamic control systems that smooth rapid changes in power demand and improve grid resilience.

## Methods

The project will be completed through the following stages:

1. **Literature Review**

   * Study the Duck Curve and grid ramp-rate challenges.
   * Learn the fundamentals of battery energy storage and grid operation.
   * Review numerical differentiation, numerical integration, and optimization techniques.

2. **Mathematical Modeling**

   * Represent electrical demand and solar generation as time-series functions.

   * Compute net load:

     $$
     N(t)=D(t)-S(t)
     $$

   * Estimate the derivative (ramp rate) using finite differences.

   * Estimate battery energy using numerical integration over discrete time intervals.

3. **Simulation Development**

   * Develop a Python simulation that processes time-series data.
   * Implement a battery controller that charges or discharges whenever the net-load ramp exceeds a specified threshold.
   * Track battery state of charge while enforcing physical limits (0%–100% capacity).

4. **Optimization**

   * Repeatedly simulate different battery capacities.
   * Identify the minimum battery size that maintains ramp-rate constraints throughout the simulation.

5. **Analysis**

   * Compare grid behavior with and without battery control.
   * Evaluate how battery size influences grid stability and energy usage.
   * Discuss assumptions, limitations, and possible improvements.

## Data Plan

The project will begin using a synthetic Duck Curve dataset generated from mathematical demand and solar-production models. This allows the computational methods to be developed and validated in a controlled environment.

If time permits, the simulation will then be tested using publicly available electrical demand and solar generation data from Texas or other regions with significant solar generation. The data will be processed into uniform time intervals suitable for numerical analysis.

## Expected Outcomes

The final deliverables of this project will include:

* A mathematical model describing net electrical load.
* A Python simulation implementing numerical differentiation, numerical integration, and battery control logic.
* An optimization routine that estimates the minimum battery capacity needed to satisfy ramp-rate constraints.
* Visualizations showing demand, solar generation, net load, battery state of charge, and ramp rates.
* A written report discussing the mathematical methods, computational implementation, simulation results, and implications for renewable energy integration.

It is expected that the project will demonstrate how relatively modest battery systems, when operated using mathematically informed control algorithms, can substantially reduce dangerous ramp-rate events. More broadly, this study will illustrate how computational mathematics—including numerical methods, simulation, and optimization—can provide practical solutions to modern engineering and disaster-resilience challenges.
