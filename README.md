## Hi there, I'm Wanjiru Ndung'u (Wanji) 

I'm a Data Engineer. I build the systems that sit underneath enterprise analytics pipelines, metric layers, and the infrastructure that turns messy source data into something teams can actually trust.
Most of what I do is unglamorous: cleaning up fragmented data, making sure definitions are consistent across systems, and building transformations that don't break when something upstream changes. The goal is always the same, analysis that holds up under scrutiny.

The repositories here reflect the kinds of problems I want to keep working on at a senior level: production-grade pipelines, data quality and contract frameworks, governed metric layers, forecasting workflows, and analytics infrastructure built for real business use rather than demo purposes.

### What I work on

I work across the full data layer from ingestion to the API endpoints that serve trusted metrics to downstream consumers.

In practice that means designing modular pipeline architectures with clear separation between ingestion, validation, transformation, and serving. Building data contract systems that catch source-level issues before they reach reporting. Designing metric layers where every KPI has an owner, a versioned definition, and tests. Working on reconciliation across systems that don't agree with each other. Forecasting and decision-support workflows where the engineering matters as much as the model. Experimentation infrastructure assignment, metric collection, statistical evaluation. And data products built for businesses operating across multiple markets, multiple source systems, and multiple definitions of the same thing.

## Stack

**Core:** Python, SQL & dbt are daily working tools.

**Pipelines & orchestration:** Prefect, Airflow patterns, custom Python connectors with abstract base interfaces. I lean toward Prefect for new work because it stays out of the way.

**Warehousing & transform:** DuckDB locally for fast iteration, with dbt projects structured staging → intermediate → marts. Comfortable working against Snowflake, BigQuery, or Postgres, the dbt project is the same shape regardless of where it runs.

**Cloud & platforms:** Currently extending into Azure (Fabric, Data Factory) and Salesforce Data Cloud CDP certifications in progress.

**Validation & quality:** Great Expectations, custom YAML-based data contracts, Pandera for schema validation, structured failure routing rather than silent corruption.

**Serving & observability:** FastAPI for data-as-a-product endpoints, structured logging, column-level lineage tracking, schema registries that flag upstream drift. Less interested in dashboards as outputs, more interested in APIs and trusted data layers.

**Statistical & ML:** statsmodels, scikit-learn for forecasting and experimentation. Some earlier work in R kept for statistical scripting where it still earns its place.

**Workflow:** Git, GitHub, Docker, GitHub Actions for CI, structured repositories, documentation-first delivery, Architecture Decision Records.

## Problems I find interesting

I'm drawn to environments where the data is a mess, specifically:

- Source systems that don't agree with each other, no canonical model in between
- KPIs that mean three different things depending on who you ask, and nobody owns the definition
- Manual processes that have quietly become load-bearing infrastructure
- Reports nobody trusts but everyone still uses
- A business that has outgrown its data infrastructure but hasn't admitted it yet
- multi-market or multi-entity ops where the same metric needs to mean the same thing across 12 different contexts

These are the conditions where good engineering actually matters & where most data work is still being conducted manually because no one has structured the underlying issue properly.

## How I approach them

I try to do the same things in the same order. Get the source logic clear before anything else. i get the source logic clear before anything else, what each system actually contains, where it disagrees with the others, and what the canonical model needs to look like. Define the metrics and assumptions explicitly so they're not buried in someone's spreadsheet versioned, owned, tested. Build transformations that can be tested and reused, with staging and mart layers separated cleanly. Design validation as configuration rather than code, so business rules stay readable. Keep the data layer separate from how it gets presented APIs and metric stores, not coupled dashboards. And make sure what finally comes out is technically sound and actually useful for the people making decisions, not just visually impressive.

Documentation gets written as the work happens, not after. ADRs for design decisions. Case studies for the harder problems. Future-me always needs the context.

## Themes you'll see across my repositories

Reliable transformation logic with clear lineage. Enterprise-style data modelling + staging, intermediate, marts, with metric layers on top. Governed metric stores with ownership, versioning, and tests. Data quality and observability built into the pipeline, not bolted on after. Forecasting and scenario work where the engineering is part of the deliverable. Experimentation frameworks with proper statistical foundations. Analytics that ends in a decision or an action, not just a chart.

Everything is built with production patterns even when the project is small, structured logging, retry logic, dependency separation, configuration over hardcoding, tests that actually run in CI.

## What I'm building toward

Stronger public proof in the areas I want to work in next: senior data engineering, analytics engineering, applied data science, forecasting, experimentation, governance-minded data platforms, and the data infrastructure roles in industries where the data environment is genuinely hard such as in aviation, energy, healthcare, fintech, multi-market commercial operations.

## A note on the work

Client work isn't published directly. The repositories here use recreated logic, synthetic data, or simplified versions of the kinds of problems I've worked on in production envirionments, multi-market enterprise CRM systems, fragmented source data, conflicting metric definitions, and the engineering patterns that make those environments tractable.

---

[LinkedIn](https://www.linkedin.com/in/junewanjirundungu/)

