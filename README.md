# PV LCA Optimization Engine v2.3 
### Advanced EPD Analytics & Scenario Modeling for Renewable Infrastructure

![Status](https://img.shields.io/badge/Status-Private%20%2F%20Proprietary-red)
![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![Streamlit](https://img.shields.io/badge/Frontend-Streamlit-FF4B4B)
![PostgreSQL](https://img.shields.io/badge/Database-PostgreSQL-336791)

---

## 🚀 Project Overview

The **PV LCA Optimization Engine** is a full-stack decision support tool designed to streamline the environmental assessment of photovoltaic (PV) projects. By bridging the gap between raw manufacturing specifications and strategic sustainability goals, this tool reduces complex assessment timelines by approximately **60%**.

It was engineered to solve data interoperability issues in the renewable sector, ingesting fragmented data from unorganized manufacturer PDFs and standardizing it into a normalized, search-ready asset aligned with **EPD Hub V3** and **EN 15804+A2** standards.

> **Note:** This repository serves as a **technical portfolio and documentation archive**. The source code and raw datasets are **private** due to strict non-disclosure agreements (NDAs) regarding third-party environmental databases (Environdec).

---

## 📸 Interface & Capabilities

### 1. Main Dashboard & Scenario Modeling
*Real-time calculation of GWP (Global Warming Potential) based on project location, lifetime, and technical yield.*
![Dashboard View](assets/Dashboard.png)
![Location Based Set Values for Berlin](assets/Set_Values_Location_1.png)
![Location Based Set Values for Seville](assets/Set_Values_Location_2.png)
![Location Based Set Values for Stockholm](assets/Set_Values_Location_3.png)

### 2. Trade-off Topology
*Multi-criteria decision analysis comparing Economic (LCOE), Environmental (GWP), and Technical efficiency.*
![Topology View](assets/Optimization_Goal_Selection.png)

### 3. Stochastic Risk Analysis (Monte Carlo)
*Probabilistic simulation (N=1000) to account for data uncertainty and supply chain variance.*
![Risk Analysis](assets/Stochastic.png)

---

## ⚡ Key Features

### 🔧 Data Engineering & Architecture
* **Automated Ingestion:** Python scripts with OCR capabilities to scrape and structure data from hundreds of unorganized manufacturer PDFs.
* **Normalization Logic:** rigorous algorithms to convert inconsistent industry units (e.g., per panel vs. per m²) into standardized functional units (per kWh, per kWp).
* **Relational Database:** A normalized SQL schema managing 200+ turbine/module models and 80+ location profiles.

### 📊 Simulation Engine
* **Monte Carlo Simulation:** Integrated Python libraries (`numpy`, `scipy`) to perform stochastic analysis on environmental impact data.
* **LCOE & AEP Calculation:** Automated workflows for Annual Energy Production and Levelized Cost of Energy, validated against German governmental wind/solar data.
* **Compliance:** Calculation methodologies validated against ISO 14040/44 standards.

---

## 🛠️ Technical Stack

* **Core Logic:** Python (Pandas, NumPy, SciPy)
* **Web Framework:** Streamlit (Custom components for interactive charts)
* **Database:** PostgreSQL (Hosted on AWS RDS for development)
* **Visualization:** Plotly & Matplotlib
* **Version Control:** Git

---

## 🔒 License & Access

**Copyright © 2025 [Yash Gupta]**
*The architectural design, logic, and interface concepts are intellectual property of the author. Underlying environmental datasets are licensed from Environdec and cannot be redistributed.*

For technical inquiries or a live demonstration of the sanitized sandbox environment, please contact me via [LinkedIn](https://www.linkedin.com/in/yashjgupta).
