# 40nm Low-Power ASIC Physical Design Project

## Project Overview

This project focuses on the **block-level physical design implementation of a low-power ASIC** using **40nm technology**. The design consists of multiple voltage and clock domains and was implemented using **Synopsys ICC2** for physical design and **PrimeTime** for Static Timing Analysis (STA).

## Design Specifications

* **Technology:** 40nm
* **Design Type:** Block-Level ASIC
* **Voltage Domains:** 9 Multi-VDD domains
* **Clock Domains:** 4
* **Standard Cells:** ~48K
* **Macros:** 34
* **Clock Frequency:** 1 GHz
* **Metal Layers:** 7
* **Cell Types:** LVT, NVT, HVT

## Physical Design Flow

The project followed the complete RTL-to-GDSII physical design flow:

1. **Floorplanning**

   * Defined core and die area
   * Placed macros considering timing and congestion
   * Created placement blockages and keepout regions
   * Performed power-aware floorplanning for multiple voltage domains

2. **Power Planning**

   * Created power and ground networks
   * Implemented power rings, straps, and rails
   * Analyzed IR drop and addressed power integrity issues
   * Checked and resolved related DRC violations

3. **Placement**

   * Performed standard-cell placement and optimization
   * Analyzed and reduced placement congestion
   * Fixed transition and setup timing violations
   * Addressed multi-voltage related violations

4. **Clock Tree Synthesis**

   * Implemented **Classic and CCD CTS flows**
   * Optimized clock latency and skew
   * Fixed clock transition violations
   * Resolved post-CTS hold timing violations

5. **Routing**

   * Performed global and detailed routing
   * Analyzed routing congestion
   * Resolved routing-related DRC violations
   * Optimized critical nets for timing closure

6. **Static Timing Analysis**

   * Performed setup and hold timing analysis using PrimeTime
   * Analyzed timing paths and slack
   * Performed timing optimization and closure
   * Worked with timing constraints and multiple operating conditions

## Key Challenges Addressed

* Multi-VDD implementation challenges
* Congestion management
* IR drop and power integrity issues
* Transition violations
* Setup and hold violations
* Clock skew and latency optimization
* Routing DRC violations
* Multi-voltage design rule violations

## Tools & Technologies

* **Synopsys ICC2** – Physical Design
* **Synopsys PrimeTime** – Static Timing Analysis
* **40nm CMOS Technology**
* **Multi-VDD / Low-Power Design**
* **LVT / NVT / HVT Standard Cells**
* **ASIC Physical Design Flow**

## Key Learning

This project provided hands-on exposure to **low-power ASIC physical design**, including power-aware floorplanning, multi-voltage implementation, placement optimization, CTS, routing, timing analysis, and timing closure.
