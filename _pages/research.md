---
title: "DIGEST Project - Research"
layout: textlay
excerpt: "DIGEST -- Research"
sitemap: false
permalink: /research/
---

# Research

## Summary
DIGEST focuses on the integration of grid energy storage into the grid. Specifically, the project aims to demonstrate the carbon emissions savings possible by optimally locating and operating storage to avoid curtailment of renewables and additional fossil fuel generation. Energy storage can provide many benefits to the power grid, and it is projected that substantial storage will be required to meet UK net-zero targets (Aunedi 2021). However, it is not clear whether the financial and environmental advantages of storage currently align (e.g., if storage is placed far from excess renewable generation, on the other side of a congested network).

The DIGEST project aims to test two hypotheses:

1. that carbon emission benefits occur if the location-specific impacts of storage during dispatch are accounted for;
2. that optimal placement of storage in the network enables substantially accelerated deployment of clean energy generators.
To explore these, we have developed novel GB transmission grid and market models, and are simulating two scenario groups. First, what are the emissions impacts of existing and soon-to-be-built storage, and how could emissions be reduced? Second, how will emissions evolve over the next 15 years considering planned generation, storage, upgrades, and new demand.

## Objectives

DIGEST has five key objectives, structured into four work packages:

<p align="center">
  <img alt="DIGEST project work package structure" src="{{ site.url }}{{ site.baseurl }}/images/respic/WP_structure.svg" width="70%">
  <br>
    <em>Figure 1. Work packages</em>
</p>

1. Develop a high-fidelity GB transmission system power flow and market model which can be used to evaluate the direct and indirect carbon impacts of new grid-scale energy storage systems, accounting for technology and location.
2. Develop scenarios for assessing the carbon reduction potential of energy storage at investment/planning time scales and methods for quantifying the impact of energy storage investment decisions on system-level carbon and financial performance.
3. Develop new tools for time series modelling and data curation, generation, and management to improve model consistency and to accurately quantify the uncertainty of results.
4. Complete national scale analysis for the next 15 years and develop a report with policy recommendations for near- and longer-term market reforms.
5. Integrate the new models into an open-source software toolkit for other researchers, analysts, and policymakers.

## Models

DIGEST advances and links leading GB national network models:

### High-fidelity short-term model 

Thomas Morstyn and team have developed a high-fidelity 2000 node GB transmission network model integrated with a Balancing Mechanism market model and Elexon unit-level data.

<p align="center">
  <img alt="DIGEST project Edinburgh UK grid model" src="{{ site.url }}{{ site.baseurl }}/images/respic/emissions.png" width="60%">
  <br>
    <em>Figure 2. Cost and carbon implications of deploying additional wind capacity in different locations on the GB grid</em>
</p>


### Long-term model 

Marko Aunedi and team are using an established whole-electricity system model to quantify cost implications across different segments of electricity system using mixed integer linear programming. As part of this project this will be extended to represent the GB transmission network with a higher granularity. 

<p align="center">
  <img alt="DIGEST project Imperial College UK grid model" src="{{ site.url }}{{ site.baseurl }}/images/respic/WeSIM_nodes.png" width="50%">
  <br>
    <em>Figure 3. 37 nodes for location specific assessment of storage on the GB grid</em>
</p>


### References

Aunedi, Wills, Strbac, Green, [“Net-zero GB electricity: cost-optimal generation and storage mix”](https://www.imperial.ac.uk/energy-futures-lab/reports/white-papers/net-zero-gb-electricity/), Energy Futures Lab White Paper, June 2021.
