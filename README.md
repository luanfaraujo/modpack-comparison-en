# Comparative Analysis of Software Feature Bundles
An independent project whose ultimate aim was to inform a team decision about choosing the best feature bundle (modpack) for the team's needs. Project done mainly using Microsoft Excel.

_Se preferir a versão em Português deste projeto, [clique aqui](https://github.com/luanfaraujo/modpack-comparison-ptbr)._

---

## Overview

This project demonstrates how structured data analysis can support decision-making when comparing multiple alternatives with overlapping features. The dataset consists of six distinct software feature bundles (sourced from JSON via an API). The goal was to determine how the bundles differ in content, where they overlap, and which option best fits the needs of the end users.

Although the dataset here comes from a **game modpack API**, the process mirrors real-world business scenarios such as comparing SaaS subscription tiers, vendor offerings, or product bundles.

---

## Objectives

- Extract and consolidate feature lists from multiple bundles.
- Clean and structure the data for consistent comparison.
- Categorize features into functional groups (e.g., Utility, Performance, Visuals).
- Enable side-by-side analysis of bundle content and distribution by category.
- Provide decision support for selecting the most appropriate bundle.

---

## Process

1. Data Extraction

- Retrieved feature lists in JSON format via API.
- Imported raw data into Excel using PowerQuery.

2. Data Transformation

- Cleaned and standardized the raw inputs.
- Retained only relevant attributes (id, name, description, URL).
- Combined all four bundles into a masterlist, with an additional column identifying the originating bundle.

3. Feature Engineering

- Created a catalog sheet to remove duplicates and assign each feature to a category (e.g., Combat, Magic, Cosmetic, Bugfix, Utility, Library).
- Used XLOOKUP to enrich the masterlist by mapping categories automatically.

4. Analysis

- Built PivotTables to quantify category distribution across bundles.
- Applied filters to identify specific categories of interest (e.g., which bundles had the most “Magic” features).
- Compared overlapping vs. unique features across bundles.

---

## Results & Insights

- Generated clear breakdowns of category distribution per bundle, showing which bundles emphasized specific types of features.
- Identified overlapping features that appeared across multiple bundles as well as unique differentiators.
- Enabled faster, evidence-based selection of the most suitable bundle based on group preferences.

---

## Tools & Skills Demonstrated

- **Data Acquisition:** API / JSON extraction
- **Data Transformation:** PowerQuery (ETL principles)
- **Data Enrichment:** Feature categorization, XLOOKUP mappings
- **Analysis:** PivotTables, filtering, comparative breakdowns
- **Decision Support:** Structured insights for evaluating multiple alternatives
