# Hospital Management Dashboard

A comprehensive Power BI report that visualizes and analyzes key metrics for hospital operations, patient flow, and resource utilization. This project demonstrates best practices in data modeling, DAX calculations, and interactive dashboard design to support data-driven decision making in healthcare management.

---

## Table of Contents

1. [Project Overview](#project-overview)  
2. [Key Features](#key-features)  
3. [Data Sources & Model](#data-sources--model)  
4. [File Structure](#file-structure)  
5. [Prerequisites](#prerequisites)  
6. [Installation & Setup](#installation--setup)  
7. [Usage](#usage)  
8. [Contributing](#contributing)  
9. [License](#license)

---

## Project Overview

This repository contains the Power BI report file (`Hospital Management Project Final 2.pbix`) that delivers:

- **Operational Insights:** Bed occupancy rates, admission and discharge trends, average length of stay.  
- **Financial Performance:** Revenue analysis by department, cost-per-patient calculations, payer mix breakdown.  
- **Resource Utilization:** Staffing levels, equipment usage rates, supply consumption patterns.  

An executive dashboard and several detailed report pages guide stakeholders through interactive visuals, enabling drill-through and cross-filtering across dimensions such as department, physician, diagnosis, and time period.

---

## Key Features

- **Interactive Executive Summary:** KPI cards, trend lines, and gauge visuals highlighting patient volume, revenue, and average LOS (Length of Stay).  
- **Departmental Drill-Downs:** Detailed pages for Admissions, Discharges, Financials, and Resource Utilization, with slicers for date, department, and patient demographics.  
- **Advanced DAX Measures:**  
  - Rolling 12-month averages  
  - Year-over-Year growth  
  - Dynamic ratio and ranking calculations  
- **Data Refresh Automation:** Configured queries to pull from source tables (CSV/SQL Server) with Power Query transformations for cleaning and standardization.  
- **Responsive Layout:** Designed for desktop and tablet viewing, with mobile-optimized bookmarks.

---

## Data Sources & Model

| Table Name         | Description                                     |
| ------------------ | ----------------------------------------------- |
| `Admissions`       | Patient admission records (date, department, DRG) |
| `Discharges`       | Patient discharge details (length of stay, outcome) |
| `Financials`       | Billing and revenue data by service line         |
| `Staffing`         | Employee rosters, shifts, and cost rates         |
| `Inventory`        | Medical supply and equipment usage logs         |

Relationships have been configured in the data model to link fact tables (`Admissions`, `Discharges`, `Financials`) to dimension tables (`Date`, `Department`, `Physician`, `Patient Demographics`).
