# FX-Trade-Lifecycle-Management-Controls-Automation-System
A full end-to-end simulation of institutional FX post-trade operations including aggregation, allocation, matching, cancel/rebook, rollovers, exception handling, and regulatory controls.

## Overview
This project is a complete simulation of an institutional FX Operations environment, designed to replicate the responsibilities of a Securities & Derivatives Analyst in a real post-trade operations setting.
It models the entire FX trade lifecycle, including:
- Trade Capture
- Aggregation
- Allocation
- Matching
- Cancel & Rebook
- Rollovers & Early Pickup/Utilization
- Regulatory & Compliance Controls
- Exception Identification, Escalation & Workflow Management
- Operational Dashboards

The system demonstrates how FX Operations teams ensure trade accuracy, minimize operational risks, manage lifecycle events, and maintain compliance with internal and external regulations.


## Project Objectives
- Simulate real-world FX post-trade workflows from capture to settlement.
- Build a control framework to detect mismatches, exceptions, and operational risks.
- Implement escalation logic with audit trails for transparency.
- Provide a dashboard for operational monitoring, compliance alerts, and KPIs.
- Create a modular, extendable codebase that mirrors institutional architecture.


## Context
In investment banks, FX Operations teams support the Front Office by ensuring:
- Trades are captured correctly
- Lifecycle events (rollovers, rebooks) are processed
- Mismatches are identified and resolved
- Clients are allocated correctly
- Regulatory controls (EMIR, FATCA, AML) are adhered to
- Exceptions are escalated and resolved on time
This project demonstrates all of these responsibilities.

## Features

1️⃣ Trade Capture
- Parses CSV trades from Sales/Trading
- Validates required fields
- Normalizes formats
- Applies client-level rules

2️⃣ Trade Aggregation

Aggregates trades based on:
- Client
- Currency pair
- Settlement date
- Product type (spot/forward/swap)
- Improves operational efficiency and reduces processing load.

3️⃣ Allocation Engine

Allocates aggregated orders:
- Based on client instructions
- Using proportionate, preset, or rule-based splits
- Captures exceptions (invalid accounts, mismatched positions)


4️⃣ Trade Matching (STP / CTM Simulation)
- Compares internal vs client trade economics
- Flags mismatches:
- Notional
- Rate
- Currency
- Settlement date
- Assigns owners and escalates breaks


5️⃣ Cancel & Rebook Workflow
- Cancel incorrect trades
- Auto-create rebooked trades
- Ensures audit trails
- Tracks who/why/when


6️⃣ Rollover & Early Pickup / Utilization
- Rollover forward legs
- Update swap points
- Validate credit utilization
- Flag early pickup scenarios


7️⃣ Compliance & Regulatory Controls

Includes:
- FATCA / EMIR field validation
- Off-market rate detection
- AML rule checks
- Mandated reporting flags
- Completion SLA validation


8️⃣ Exception Manager
- Logs all mismatches/breaks
- Assigns responsibility
- Tracks ageing
- Performs escalations
- Generates final reports


9️⃣ Dashboard (Using Streamlit)

Displays:
- Trades pending match
- Allocation exceptions
- Cancel/rebook status
- Compliance violations
- Daily operational KPIs

## Trade Lifecycle Flow (High-Level Diagram)

    Trade Capture → Validation → Aggregation → Allocation → Matching →
    Cancel/Rebook → Rollover/Early Pickup → Compliance Checks →
    Exceptions → Escalation → Dashboard Reporting

## Use Cases Demonstrated

This project directly showcases competency in:
- Post-trade operational processes
- FX trade lifecycle management
- Control & risk frameworks
- Exception handling
- Stakeholder coordination
- Regulatory compliance awareness
- Data cleaning, transformation, and reporting
- Written/visual communication of financial workflows
