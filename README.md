# Bolted Joint Calculator

**A robust, open-source engineering tool for the analysis and design of bolted joints.** This calculator empowers engineers, designers, and students to perform critical calculations for verifying the integrity, safety, and optimal performance of bolted connections under various mechanical loads.

---

## Overview

Bolted joints are ubiquitous in mechanical systems, from automotive to heavy machinery. This project automates the complex calculations required to ensure their reliability, minimizing design errors and optimizing material use. It handles various load cases and evaluates safety against common failure modes according to established engineering standards.

---

## Features

*   **Comprehensive Analysis:** Calculates preload, stresses (tensile, shear, combined), and safety factors against yield, ultimate, and fatigue failure.
*   **Multi-Standard Support:** Implements calculations based on industry standards like VDI 2230, ASME, and ISO.
*   **Flexible Inputs:** Supports both SI (Metric) and US Customary units, with options for various bolt grades and joint materials.
*   **Dynamic & Static Loads:** Handles both static and dynamic/fatigue loading conditions.
*   **Torque Recommendations:** Provides recommended tightening torques for desired preload.
*   **Interactive & Batch Processing:** Offers both a command-line interface (CLI) for quick calculations and a planned graphical user interface (GUI) or web interface for comprehensive analysis.

---

## Installation

### Requirements

*   Python 3.8+
*   `pip` (Python package installer)

### Steps

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/lukeholste/bolted-joint-calculator.git
    cd bolted-joint-calculator
    ```
2.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

---

## Quick Start (CLI)

Perform a basic analysis for an M16 Grade 8.8 bolt under a 50 kN tensile load:

```bash
python -m bolted_joint_calculator \
  --bolt-grade "8.8" \
  --bolt-diameter 16 \
  --bolt-count 4 \
  --grip-length 25 \
  --tensile-load 50000 \
  --unit metric
