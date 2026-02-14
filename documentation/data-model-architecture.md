# Data Model Architecture

## Model Overview

A simplified star schema was implemented to ensure analytical consistency and scalability.

**Fact Table:** `Operations_Data`  
**Dimension Table:** `Date`


## Fact Table – Operations_Data

**Granularity:** One row per logistics event.

Contains operational metrics such as:

- `event_type`
- `location_state`
- `delivery_delay_minutes`
- `detention_minutes`
- `Scheduled_Date`
- `DateOnly`

Serves as the primary source for KPI calculations.


## Dimension Table – Date

A dedicated calendar table was created to enable proper time intelligence.

Derived columns:

- `Year`
- `YearMonth`
- `YearMonthSort`


## Relationship Design

- `Date[Date]` → `Operations_Data[DateOnly]`
- Cardinality: **1-to-Many (1:*)**
- Cross-filter direction: **Single**

This structure ensures:

- Accurate time-based aggregation
- Proper chronological sorting
- Clean separation between fact and dimension tables
- Prevention of ambiguous filter propagation


## Modeling Principles Applied

- Star-schema logic  
- Explicit calendar dimension  
- Single-direction filtering  
- Defined data granularity  
- Business logic implemented through DAX measures  


## Scalability Considerations

The model supports future expansion, including:

- Additional dimensions (Facility, Customer, Carrier)
- Advanced time intelligence (MoM / YoY)
- SLA segmentation by region or client
- Forecasting extensions
