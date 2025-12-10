# Power BI Model Documentation Guide

This guide explains how to use the Excel macro-enabled documentation file, which contains comprehensive technical documentation of the Power BI data model.

---

## What is This File?

This Excel workbook (.xlsm) provides detailed technical documentation of the Power BI data model, including:

- Complete data model structure and table relationships
- All DAX measures with full formulas and display folders
- Column-level details (data types, cardinality, sizes)
- Model performance metrics and memory usage
- Relationship definitions and cardinality ratios

This documentation serves as a reference for developers, analysts, and stakeholders to understand the model's technical implementation.

---

## Prerequisites

**System Requirements:**
- Microsoft Excel 2016 or later (Windows or Mac)
- Macros must be enabled for full functionality

---

## How to Open the File

1. **Download** the Excel documentation file (.xlsm) to your computer
2. **Open** the file in Microsoft Excel
3. **Enable macros** when prompted by clicking "Enable Content" in the security warning banner
4. **Navigate** between worksheet tabs to explore different aspects of the model

---

## What's Inside

The documentation file typically contains the following sections organized as Excel worksheets:

### Summary Sheet
High-level overview of the data model:
- Total file size and last refresh date
- Number of tables, measures, and columns
- Model complexity metrics
- Key statistics at a glance

### Tables Sheet
Detailed table-level information:
- Table names and row counts (cardinality)
- Total data size per table
- Number of columns and relationships
- Partitioning and segment information

### Columns Sheet
Column-level breakdown:
- Column names, data types, and cardinality
- Memory usage and compression statistics
- Hierarchies and relationships
- Dictionary sizes and encoding

### Measures Sheet
Complete DAX measure library:
- Measure names and display folders
- Full DAX expressions and formulas
- Format strings and descriptions
- Hidden/visible status

### Relationships Sheet
Model relationship definitions:
- Source and target tables/columns
- Relationship type (1:1, 1:Many, Many:1)
- Cardinality ratios and filter direction
- Cross-filter settings

### Data Types Sheet
Memory allocation by data type:
- Boolean, DateTime, Integer, String, etc.
- Database size percentage per type
- Row count and memory distribution

---

## How to Use This Documentation

### For Developers
- **Review DAX logic**: Examine measure formulas to understand business logic and calculation methods
- **Validate relationships**: Verify proper table connections and filter propagation
- **Optimize performance**: Identify large columns or tables for compression and indexing improvements
- **Debug issues**: Reference exact formulas when troubleshooting calculation errors

### For Business Analysts
- **Understand metrics**: See how KPIs and measures are calculated
- **Reference measure names**: Find exact measure names for report building
- **Explore data structure**: Understand which tables contain what information
- **Verify calculations**: Confirm business logic implementation

### For Stakeholders
- **Model transparency**: Gain visibility into data model complexity and structure
- **Quality assurance**: Review calculations for accuracy and business alignment
- **Documentation**: Use as technical reference for audits and governance

---

## Updating the Documentation

This documentation file is generated from the Power BI model and should be refreshed when significant model changes occur:

- After adding/modifying DAX measures
- When restructuring table relationships
- Following major data model updates
- Before major releases or audits

**Note:** The specific method for regenerating this file depends on the tool used (e.g., DAX Studio, Tabular Editor, custom export scripts). Consult your BI development team for the refresh process.

---
