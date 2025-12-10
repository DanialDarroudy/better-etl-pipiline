# Better ETL Pipeline – CSV to PostgreSQL with APIs

A robust C# ETL (Extract, Transform, Load) pipeline that converts CSV data into PostgreSQL with advanced aggregation and conditional queries.  
Built with modern design patterns, connection pooling, and observability via OpenTelemetry. Includes APIs for flexible integration and comprehensive unit testing.

---

## 🚀 Features
- **CSV → PostgreSQL conversion** with schema mapping  
- **Aggregation & conditional queries** with query generator  
- **Adapter & Factory patterns** for flexible data source integration  
- **Connection pool** for efficient database access  
- **Three APIs**:
  - Aggregate query API  
  - Condition query API  
  - CSV import API  
- **OpenTelemetry logging** for observability and monitoring  
- **FluentValidation** for input validation  
- **Unit tests** with xUnit, FluentAssertions, and NSubstitute for mocking  

---

## 🏗️ Architecture Overview
- **Extract Layer**
  - Reads CSV files via Adapter pattern
  - Factory pattern for dynamic instantiation of extractors

- **Transform Layer**
  - Query generator for aggregation and condition queries
  - FluentValidation for data validation

- **Load Layer**
  - Connection pool for efficient PostgreSQL inserts
  - Batch loading with error handling

- **API Layer**
  - REST endpoints for aggregate queries, condition queries, and CSV import

- **Testing Layer**
  - Unit tests with xUnit
  - FluentAssertions for expressive validation
  - NSubstitute for mocking dependencies

---

## 🛠️ Technologies
- C# (.NET Core)  
- PostgreSQL  
- CSV parsing  
- Adapter & Factory design patterns  
- Connection pooling  
- OpenTelemetry (OTel) for logs  
- FluentValidation  
- xUnit + FluentAssertions + NSubstitute  
