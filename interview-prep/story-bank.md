# Story Bank — Master STAR+R Stories

This file accumulates your best interview stories over time. Each evaluation (Block F) adds new stories here. Instead of memorizing 100 answers, maintain 5-10 deep stories that you can bend to answer almost any behavioral question.

## How it works

1. Every time `/career-ops oferta` generates Block F (Interview Plan), new STAR+R stories get appended here
2. Before your next interview, review this file — your stories are already organized by theme
3. The "Big Three" questions can be answered with stories from this bank:
   - "Tell me about yourself" → combine 2-3 stories into a narrative
   - "Tell me about your most impactful project" → pick your highest-impact story
   - "Tell me about a conflict you resolved" → find a story with a Reflection

## Stories

<!-- Stories will be added here as you evaluate offers -->
<!-- Format:
### [Theme] Story Title
**Source:** Report #NNN — Company — Role
**S (Situation):** ...
**T (Task):** ...
**A (Action):** ...
**R (Result):** ...
**Reflection:** What I learned / what I'd do differently
**Best for questions about:** [list of question types this story answers]
-->

### [Platform] Snowpipe micro-batch migration
**Source:** Report #001 — Microsoft — Data Engineer II
**S (Situation):** A $100B+ financial institution had a 4-hour nightly delay before risk dashboards were fresh enough to use.
**T (Task):** Cut latency materially without breaking existing reporting dependencies.
**A (Action):** Re-architected batch ingestion into a Snowflake Snowpipe micro-batch flow on AWS using S3, CloudFormation, and Airflow.
**R (Result):** Delivered sub-10-minute freshness across 15+ executive risk and compliance dashboards.
**Reflection:** Platform work only matters when it changes the consumer experience; freshness is a product requirement, not a technical vanity metric.
**Best for questions about:** most impactful project, reliability, handling ambiguity, production pipelines

### [Governance] Data contracts and ownership model
**Source:** Report #001 — Microsoft — Data Engineer II
**S (Situation):** Downstream data issues were recurring because ownership and data behavior were not explicit enough.
**T (Task):** Establish a more durable operating model across engineering, risk, compliance, and data science.
**A (Action):** Defined data contracts, pipeline SLAs, and schema governance standards across teams.
**R (Result):** Reduced downstream data issues and created a clearer ownership model for production data.
**Reflection:** Governance works best when it is built into the operating model early instead of being bolted on after incidents.
**Best for questions about:** conflict resolution, cross-functional work, governance, leadership

### [Azure] Latency reduction on ADF and Synapse
**Source:** Report #001 — Microsoft — Data Engineer II
**S (Situation):** BI consumers were waiting 6 hours for refreshed data, which slowed business decisions.
**T (Task):** Modernize the pipeline and enable faster consumption for stakeholders.
**A (Action):** Built ELT pipelines with Azure Data Factory, PySpark, Databricks, Synapse, and Python.
**R (Result):** Reduced data delivery latency by 92% and enabled 8 BI teams to work with near-real-time data.
**Reflection:** The best modernization work removes manual dependency chains and makes the platform easier to operate.
**Best for questions about:** modernization, Azure, stakeholder impact, execution speed

### [Analytics] Medallion lakehouse for self-service reporting
**Source:** Report #001 — Microsoft — Data Engineer II
**S (Situation):** Finance, Operations, and Sales teams needed self-service analytics without constant engineering intervention.
**T (Task):** Provide curated, trustworthy data layers that business users could actually consume.
**A (Action):** Designed bronze/silver/gold medallion layers and SCD models in Azure Databricks and Synapse.
**R (Result):** Enabled self-service analytics for 20+ stakeholders and removed a 2-day manual reporting cycle.
**Reflection:** Curated data models are as much about user trust and usability as they are about architecture.
**Best for questions about:** data modeling, BI, stakeholder management, analytics engineering

### [Streaming] Kafka and Flink low-latency pipeline
**Source:** Report #001 — Microsoft — Data Engineer II
**S (Situation):** Distributed web log data needed to be processed in near real time for downstream use.
**T (Task):** Build a streaming pipeline with sub-2-minute end-to-end latency.
**A (Action):** Tuned Kafka topic partitioning, consumer groups, and Flink window configuration.
**R (Result):** Achieved sub-2-minute latency while maintaining zero data loss.
**Reflection:** Streaming systems reward careful tuning of the consumer SLA and failure model, not just raw throughput.
**Best for questions about:** streaming, low latency, resilience, technical depth

### [Observability] Pipeline anomaly detection and drift monitoring
**Source:** Report #001 — Microsoft — Data Engineer II
**S (Situation):** Schema drift and data quality failures were surfacing too late in daily pipeline runs.
**T (Task):** Catch bad data before it became a production incident.
**A (Action):** Built anomaly detection and monitoring for 50+ daily pipeline executions.
**R (Result):** Reduced incident response time and improved visibility into pipeline health.
**Reflection:** Observability is a leading indicator of trust; once teams see failures earlier, they make better operational decisions.
**Best for questions about:** debugging, quality, observability, learning from failure
