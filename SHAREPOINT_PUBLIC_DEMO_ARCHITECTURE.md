# Architectonic SharePoint Public Demo Architecture

**Version:** 0.1  
**Status:** PUBLIC DEMO DESIGN — SYNTHETIC ONLY

## Purpose

Provide a SharePoint-based public demonstration environment for Architectonic that is safe to inspect, easy to understand, and structurally representative without exposing proprietary Enterprise implementation, private methods, client information, restricted data, or production controls.

## Demo site

**Site:** Architectonic Community Demo

### Libraries
1. 01_Getting_Started
2. 02_Synthetic_Evidence
3. 03_Demo_Architecture
4. 04_Demo_Decision_Packages
5. 05_Demo_Measures
6. 06_Demo_Lessons

### Demo Lists
- Demo Pilot Registry
- Demo Stakeholder Register
- Demo Decision Register
- Demo Evidence Register
- Demo Architecture Nodes
- Demo Architecture Edges
- Demo Measure Register
- Demo Forecast Register
- Demo Outcome Register
- Demo QAQC Findings

## Allowed content

- synthetic Northstar Manufacturing data;
- public schemas;
- public documentation;
- simplified ontology vocabulary;
- example decision packages;
- public MOP/MOE/KPI structures;
- demonstration workflows;
- public release notes;
- public design-partner information.

## Prohibited content

- client data;
- nonpublic government information;
- credentials or secrets;
- private prompts or orchestration;
- full template library;
- private calibration data;
- benchmark assets;
- customer connectors;
- production security configurations;
- regulated deployment profiles;
- proprietary human-systems, negotiation, or advantage models;
- internal commercial or pricing logic.

## Demo workflow

SYNTHETIC INTAKE -> SYNTHETIC BASELINE -> DEMO ARCHITECTURE -> DEMO DECISION PACKAGE -> DEMO MEASUREMENT -> DEMO LESSONS

No public demo workflow may create or modify an Enterprise authoritative record.

## Demonstration views

- Executive Overview
- Architecture Graph Summary
- Decision Trace
- Evidence-to-Decision Traceability
- Measures Dashboard
- Synthetic Forecast vs Outcome
- QAQC and Abstention Examples
- Community vs Enterprise Boundary

## Public interpretation rule

Every view and artifact must state that the data is synthetic and the environment is a demonstration. The public demo does not establish production readiness, certification, field calibration, client outcomes, or autonomous decision authority.

## SharePoint boundary

A public demo site may be implemented on a separately governed SharePoint environment or site collection. Public access, anonymous access, or external sharing must follow the actual tenant's sharing policy and security configuration. This document does not assert that anonymous/public SharePoint access is available in any specific tenant.
