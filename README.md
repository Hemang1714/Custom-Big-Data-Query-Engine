# Custom Big Data Query Engine for Taxi Trip Analytics 🚖📊

A high-performance Java solution for processing 20M+ taxi trip records with custom JSON parsing and in-memory query execution.

## 🚀 Key Features
- **Custom-built query engine** (no Spark/Pandas/DuckDB)
- Processes **20M+ records** in Newline-Delimited JSON format
- Supports:
  - Filtering (`WHERE` conditions)
  - Projection (column selection)
  - Aggregation (`COUNT`, `SUM`, `AVG`, `MIN`, `MAX`)
  - Group-By operations
- **Single-pass processing** optimization
- Memory-efficient design using Java Collections

## 📋 Dataset Schema
```json
{
  "tpep_pickup_datetime": "timestamp",
  "tpep_dropoff_datetime": "timestamp",
  "VendorID": "int",
  "passenger_count": "int",
  "trip_distance": "double",
  "payment_type": "int",
  "fare_amount": "double",
  "tip_amount": "double",
  "store_and_fwd_flag": "char"
}
