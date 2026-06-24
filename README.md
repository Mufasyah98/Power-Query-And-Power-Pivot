Variance Sales :=
VAR CY =
    [Total Revenue]
VAR PY =
    CALCULATE(
        [Total Revenue],
        FILTER(
            ALL('Calendar'),
            'Calendar'[Year] = MAX('Calendar'[Year]) - 1
                && 'Calendar'[Month No] = MAX('Calendar'[Month No])
        )
    )
RETURN
    IF(
        ISBLANK(PY),
        BLANK(),
        CY - PY
    ) i'm

## Upload your assessment here

https://forms.gle/paeV5UdeGAay8Efw9

## Group telegram support

https://t.me/+j3o-Hct3ae1jYTVl




## Introduction

This repository contains resources, examples, and best practices for **Power Query** and **Power Pivot** — two powerful data transformation and modeling tools in Microsoft Excel.

### Power Query
- Used for **data extraction, transformation, and loading (ETL)**.
- Supports importing data from multiple sources (Excel, CSV, databases, web, APIs, etc.).
- Allows **data cleaning, shaping, and automation** without manual repetition.

### Power Pivot
- Used for **data modeling and advanced calculations**.
- Creates **relationships between tables** to build robust data models.
- Supports **DAX (Data Analysis Expressions)** for powerful measures and calculated columns.

### Why Use Them Together?
- Connect to diverse data sources.
- Clean, transform, and prepare data efficiently.
- Build analytical models for reporting and dashboards.
- Enable **self-service business intelligence** in Excel.
