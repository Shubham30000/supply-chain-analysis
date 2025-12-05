# Supply Chain Analytics: Correlation Matrix

**Author:** 23f2005282@ds.study.iitm.ac.in  
**Project:** OptimalFlow Logistics - Supplier Performance Analysis

## Overview

This repository contains a comprehensive correlation analysis of supply chain metrics from 57 procurement transactions for an automotive manufacturer. The analysis identifies relationships between key performance indicators to optimize supplier selection and inventory management.

## Dataset Variables

- **Supplier_Lead_Time**: Days from order placement to delivery
- **Inventory_Levels**: Current stock quantities (units)
- **Order_Frequency**: Number of orders placed per month
- **Delivery_Performance**: On-time delivery rate (%)
- **Cost_Per_Unit**: Unit cost in dollars ($)

## Files Included

1. **README.md** - This documentation file
2. **correlation.csv** - Correlation matrix values
3. **heatmap.png** - Excel conditional formatting visualization (Red-White-Green)

## Key Findings

### Strong Correlations (>0.7)
- Variables with high positive correlation indicate they move together
- Variables with high negative correlation move in opposite directions

### Weak Correlations (<0.3)
- Variables that show little relationship
- May indicate independent factors in supply chain

## Excel Analysis Steps

### 1. Enable Data Analysis ToolPak
```
File → Options → Add-ins → Manage: Excel Add-ins → Go
Check "Analysis ToolPak" → OK
```

### 2. Generate Correlation Matrix
```
Data → Data Analysis → Correlation
Input Range: Select all 5 data columns (including headers)
☑ Labels in first row
Output Range: New Worksheet
```

### 3. Apply Conditional Formatting
```
Select correlation values (exclude labels)
Home → Conditional Formatting → Color Scales
Choose: Red - White - Green
Red = Low/Negative correlation
White = No correlation
Green = High/Positive correlation
```

### 4. Export Results
- Save correlation matrix as CSV
- Screenshot heatmap (400x400 to 512x512 pixels)

## Interpretation Guide

**Correlation Coefficient Ranges:**
- **0.9 to 1.0**: Very strong positive correlation
- **0.7 to 0.9**: Strong positive correlation
- **0.5 to 0.7**: Moderate positive correlation
- **0.3 to 0.5**: Weak positive correlation
- **-0.3 to 0.3**: Little to no correlation
- **-0.5 to -0.3**: Weak negative correlation
- **-0.7 to -0.5**: Moderate negative correlation
- **-0.9 to -0.7**: Strong negative correlation
- **-1.0 to -0.9**: Very strong negative correlation

## Business Insights

The correlation matrix helps identify:
- **Supplier Selection**: Which metrics predict delivery performance
- **Cost Optimization**: Relationship between lead time and cost
- **Inventory Planning**: How order frequency affects inventory levels
- **Risk Management**: Variables that indicate delivery issues

## Contact

For questions or additional analysis:
**Email:** 23f2005282@ds.study.iitm.ac.in

---

**Project Date:** December 2025  
**Analysis Tool:** Microsoft Excel with Data Analysis ToolPak  
**Client:** OptimalFlow Logistics
