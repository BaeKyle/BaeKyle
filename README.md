# BaeKyle

Backend engineer with 9 years of experience building enterprise applications with Java and Spring.

I focus on large-scale data processing, long-running background jobs, transactional data consistency, legacy system modernization, and operational reliability.

## Professional Focus

- Enterprise application development with Java and Spring Boot
- Large dataset processing and Excel export architecture
- Asynchronous jobs and batch processing
- Transaction design and data consistency with MyBatis and relational databases
- Modernization of legacy business systems
- Production issue analysis, performance improvement, and operational stabilization

## Featured Project

### [Enterprise Excel Export Lab](https://github.com/BaeKyle/enterprise-excel-export-lab)

A Spring Boot project that demonstrates how to handle large Excel exports without keeping a browser request open or loading the entire dataset and workbook into memory.

The project addresses practical export concerns such as JVM memory pressure, request timeouts, duplicate requests, progress visibility, cancellation, and temporary-file cleanup.

Key points:

- Background export job separated from the download request
- Streaming XLSX generation with Apache POI `SXSSFWorkbook`
- Chunked database reads with MyBatis
- Export status, progress, elapsed time, and file-size tracking
- Duplicate job prevention
- Cooperative cancellation and partial-file cleanup
- Comparison between synchronous download and asynchronous bulk export
- Portfolio-safe implementation using generated data only

[View Repository](https://github.com/BaeKyle/enterprise-excel-export-lab) · [Architecture Decisions](https://github.com/BaeKyle/enterprise-excel-export-lab/blob/main/docs/architecture-decisions.md)

## Engineering Principles

- Design for realistic data volume and failure conditions.
- Define transaction boundaries and protect data consistency.
- Make long-running operations observable and recoverable.
- Document the benefits, limitations, and evolution criteria of technical decisions.
- Extract reusable structures from repeated business requirements.
- Prefer measured results and explicit trade-offs over unsupported claims.

## Tech Stack

Java · Spring Boot · MyBatis · Oracle · Apache POI  
JavaScript · Maven · Docker · Redis
