# wta-bsci-analytics# WTA Big-Stage Closer Index (BSCI)

## What this is
A Python ETL pipeline and analytics framework built during a capstone engagement 
with the Women's Tennis Association. Developed to identify which players perform 
their best under the highest-pressure match conditions.

## The problem it solves
Traditional tennis statistics don't distinguish between early-round performance 
and results achieved in Quarterfinals, Semifinals, and Finals. BSCI fills that gap.

## Tech stack
Python · Pandas · NumPy · Plotly · Excel (multi-sheet ingestion)

## Pipeline overview
1. Load and standardize match data from two WTA datasets (5,000+ records each)
2. Filter to Singles Main Draw matches only
3. Standardize round labels across inconsistent formats
4. Build player-match long table with QF/SF/F outcomes
5. Compute weighted win rate (QF=1.5x, SF=1.7x, F=2.0x) with sample guardrails
6. Export leaderboard CSV for dashboard integration

## Key results
- Processed 5,000+ match records across 12+ data formats
- Identified meaningful divergence between overall win rate and late-round performance
- Anastasia Pavlyuchenkova: 37% overall win rate → 64% big-stage close rate

## Data note
Source data is proprietary WTA property. This repository contains the pipeline 
code and anonymized sample outputs only.
