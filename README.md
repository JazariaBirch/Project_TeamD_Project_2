# Project #2: Automation of Concrete Mix Design (NDOT)

## Client
Nebraska Department of Transportation (NDOT)

## Team
Group D- Blake Green, Ahmad Rezaie, Jazaria Birch

## Date
February 23, 2026

---

# Project Overview

This project automates the Nebraska Department of Transportation (NDOT) concrete mix design process by translating an Excel-based workflow into a structured Python program.

The objective is to replicate the engineering logic contained in the NDOT "Mix Design" Excel worksheet and generate a clearly formatted weight chart for one cubic yard of concrete.

The automation improves:
Accuracy of engineering calculations, Transparency of mix design logic, Repeatability of results, Workflow efficiency compared to manual Excel entry

---

# Method

The program preforms:

1. Cementitious material weight calculations
2. Water weight using water–cement ratio
3. Volume calculations using specific gravities
4. Air volume determination
5. Total aggregate volume calculation
6. Fine and coarse aggregate weight calculations
7. Generation of a professional weight summary

All volume calculations use:

Volume = Weight / (Specific Gravity × Unit Weight of Water)

Where unit weight of water = 62.4 lb/ft³

Total batch volume = 27 ft³ (1 cubic yard)

---

#Program Structure

The script contains:

## Defined Constants
Unit weight of water
Cubic yard volume
Default specific gravities

## Functions
water_Q() – Calculates total water weight  
volume_R() – Cement volume  
volume_S() – Fly ash volume  
volume_T() – Silica fume volume  
volume_U() – Other SCM volume  
volume_V() – Air volume  
volume_W() – Water volume  
volume_X() – Total aggregate volume  
weight_Y() – Fine aggregate weight  
weight_Z() – Coarse aggregate weight  
weight_AA() – Other aggregate weight  

Each major engineering step is implemented as a separate function to ensure clarity and modularity.

---

# How to Run the Program (Jupyter Notebook)

## Step 1: Open the Notebook

1. Download or clone this repository.
2. Open Jupyter Notebook.
3. Navigate to the project folder.
4. Open the file:
---

## Step 2: Run All Cells

At the top menu, click run
to run each cell sequentially.

---

## Step 3: Enter Inputs When Prompted

The notebook collects inputs in a step-by-step order.

When prompted, enter values directly into the input box and press Enter.
All cementitious weights must be entered in:

lb per cubic yard
Water-cement ratio must be entered as a decimal
Air content and aggregate proportions must be entered as percentages.

---

# User Guide: Sequential Input Prompts

The notebook follows this exact order:

---

## 1. Project Information
Project number
Class of concrete 

---

## 2. Cementitious Materials (lb/yd³)
Cement weight A
Fly ash weight B
Silica fume weight C
Other SCM weight D

---

## 3. Water and Air Targets
Target water-cement ratio (E)
Target air content F (%)

Water weight is automatically calculated as:

Water Weight = (Total Cementitious Weight) × (Water-Cement Ratio)

---

## 4. Aggregate Percentages (%)
Percent fine aggregate G
Percent coarse aggregate H
Percent other aggregate I

---

## 5. Specific Gravities
Cement (J)
Fly ash (K)
Silica fume (L)
Other SCM (M)
Fine aggregate (N)
Coarse aggregate (O)
Other aggregate (P)

---

# Engineering Calculations Performed

The notebook automatically calculates:
Water weight (Q)
Cement volume (R)
Fly ash volume (S)
Silica fume volume (T)
Other SCM volume (U)
Air volume (V)
Water volume (W)
Total aggregate volume (X)
Fine aggregate weight (Y)
Coarse aggregate weight (Z)
Other aggregate weight (AA)

The final total batch volume equals 27 cubic feet (1 cubic yard).

---

# Output

After all inputs are entered, the notebook prints a formatted weight summary including:
Project number
Class of concrete
Cementitious weights
Aggregate weights
Water weight

All values are displayed in pounds.
