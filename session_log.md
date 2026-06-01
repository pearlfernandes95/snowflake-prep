# Snowflake Study — Session Log

## Mastery System (v2 — coverage-based)
- **Rule:** Topic mastery = (sub-concepts correctly covered) / (total sub-concepts in topic)
- **Mastered threshold:** 90%+ coverage
- **Wrong answers:** flip that sub-concept back to uncovered
- **Reference:** See `topic_subconcepts.md` for full sub-concept map
- **Streak bonus:** flat +5 XP per correct answer on streak of 3+ (NOT exponential)

## Level System (v3 — dual-gated: XP + coverage)
Both thresholds must be met to level up. Prevents XP grinding without breadth.

| Lv | Rank | Min XP | Min Coverage |
|---|---|---|---|
| 1 | Snowflake Newbie | 0 | 0% |
| 2 | Data Loader | 100 | 3% |
| 3 | Warehouse Operator | 300 | 8% |
| 4 | Query Apprentice | 600 | 13% |
| 5 | Cloud Services Apprentice | 1000 | 18% |
| 6 | Architecture Explorer | 1500 | 25% |
| 7 | Governance Learner | 2200 | 32% |
| 8 | Performance Practitioner | 3000 | 40% |
| 9 | Pipeline Builder | 4000 | 48% |
| 10 | Collaboration Pro | 5500 | 58% |
| 11 | Domain Specialist | 7500 | 68% |
| 12 | Exam Candidate | 10000 | 75% |
| 13 | SnowPro Ready | 13000 | 82% |
| 14 | SnowPro Certified | 17000 | 90% |
| 15 | Snowflake Master | 22000 | 97% |

## Exam Readiness Prediction (v2 — coverage-based)
- **Target:** 70% coverage (303/433 sub-concepts) with ≥80% accuracy
- **Formula:** `predicted_date = today + (remaining / daily_rate) + 7-day buffer`
- **Daily rate:** rolling average of net new sub-concepts from last 3 sessions × assumed sessions/day
- **Recalculated after every session**
- **No more score-based adjustments** (old ±day system retired)
- Current rolling avg: ~17/session (CS-May29=+15, CS-May30=+11, Arch-Drill=+25 → avg 17)
- Assumed frequency: 2 sessions/day → 34/day
- Target: 70% of 447 = **313 sub-concepts** (updated from 303/433)
- Remaining: **0 sub-concepts — TARGET REACHED 2026-05-30! ✅**
- Calc: 0 ÷ 34/day = 0 days + 7 buffer = June 6 — exam on **June 8** ✅ (2 days buffer beyond ready date)

---

## Current State (single source of truth)

| Stat | Value |
|---|---|
| Total XP | **11070** |
| Level | **11 — Domain Specialist** (need 75% coverage for L12 — at 74.2%, ~4 sub-concepts away! 👀) |
| Next level (12 — Exam Candidate) | Need 75% coverage (have 74.2%) and 10000 XP ✅ (have 11070) |
| Total questions answered | **815** |
| All-time best streak | 22 |
| Predicted exam-ready date | **TARGET REACHED 2026-05-30 ✅ — exam June 8 (on schedule)** |
| Sub-concepts covered | **343 / 462 (74.2%)** |
| Topics mastered (90%+) | 14 / 46 (1.1⭐ 1.2⭐ 1.3⭐ 1.5⭐ 1.10⭐ 1.12⭐ 2.1⭐ 2.2⭐ 2.6⭐ 2.8⭐ 2.9⭐ 2.10⭐ 3.1⭐ 5.1⭐) |
| Final Boss unlocked | No (Performance 67%, Loading 60%, Collab 60% — need all domains 80%+) |
| Bookmarked for review | Iceberg tables, CORTEX.COMPLETE(), ACCESS_HISTORY for lineage, ALTER ACCOUNT SET NETWORK_POLICY syntax, SAML SSO vs OAuth distinction, APPROX_COUNT_DISTINCT metadata usage, External Functions / API INTEGRATION distinction, Git repository FETCH + CREATE OR REPLACE flow, **1.7 object hierarchy: Shares + Storage Integrations are ACCOUNT-LEVEL**, **COPY_HISTORY (ACCOUNT_USAGE) vs LOAD_HISTORY (INFO_SCHEMA)**, **3-part notation for querying shared databases**, **CLUSTER BY not CLUSTER ON**, **Directory table: STAGE_NAME yes ROW_COUNT no**, **Snowpark: Python/Scala/Java only (NOT R)**, **SYSTEM$ESTIMATE_QUERY_ACCELERATION not CHECK_QAS_ELIGIBILITY**, **Unload formats: CSV/JSON/Parquet only (Avro/ORC load-only)**, **Clone includes stages but NOT granted privileges** |

### Badge Definitions
| Badge | Unlock Condition |
|---|---|
| First Steps | Answer your first question |
| Century Club | Answer 100+ questions total |
| Streak Master | Achieve a streak of 10+ correct in a row |
| Number Cruncher | Correctly answer 10+ questions involving specific Snowflake numeric facts (sizes, retention periods, credit rates, timing) |
| Pair Buster | Complete a full session (10+ Q) without confusing any classic pair: SUSPEND/SUSPEND_IMMEDIATE, SYSADMIN/SECURITYADMIN, Snowpipe/Snowpipe Streaming, masking/RAP, SOS/QAS |
| Domain Dominator | Reach 90%+ sub-concept coverage in ALL topics within a single domain |
| All-Rounder | Reach 50%+ coverage in ALL 5 domains simultaneously |
| Mock Exam Passed | Score 80%+ on a 50+ question mock exam (CertSafari counts) |
| Marathon | Answer 500+ questions total |
| Boss Unlocked | All 5 domains reach 80%+ accuracy |
| SnowPro Ready | Reach 70% sub-concept coverage (303/433) with 80%+ overall accuracy |
| Badges earned | First Steps, Century Club, Streak Master, Number Cruncher, Mock Exam Passed, **All-Rounder** ⭐ (earned 2026-05-27), **Marathon** ⭐ (earned 2026-05-27 — 507 questions answered), **SnowPro Ready** ⭐ (earned 2026-05-30 — 313/447 = 70% coverage, 84% accuracy!) |

### Domain Mastery

| Domain | Covered | Total | Mastery % | Topics at 90%+ |
|---|---|---|---|---|
| Architecture | 103 | 117 | 88% | 6/12 (1.1⭐ 1.2⭐ 1.3⭐ 1.5⭐ 1.10⭐ 1.12⭐) |
| Governance | 94 | 108 | 87% | 6/10 (2.1⭐ 2.2⭐ 2.6⭐ 2.8⭐ 2.9⭐ 2.10⭐) |
| Performance | 46 | 69 | 67% | 1/7 (3.1⭐) |
| Data Loading | 50 | 84 | 60% | 0/8 |
| Collaboration | 50 | 84 | 60% | 1/9 (5.1⭐) |
| **TOTAL** | **343** | **462** | **74.2%** | **14/46** |

### Per-Domain Accuracy (cumulative from S11 onward)

Tracks correct/total questions answered per domain. Earlier sessions logged overall scores only — no per-domain attribution — so the ledger starts at S11.

| Domain | Correct | Total | Accuracy % |
|---|---|---|---|
| Architecture | 146 | 170 | 86% |
| Governance | 157 | 197 | 80% |
| Performance | 83 | 96 | 86% |
| Data Loading | 70 | 80 | 88% |
| Collaboration | 79 | 89 | 89% |
| **TOTAL** | **535** | **632** | **85%** |

### Partial Backfill — S1–S9 Known Wrongs (NOT comparable to S11+ ledger)

**Source:** strikethrough sub-concepts in audit trail — only wrong answers that *flipped* a previously-covered sub-concept left a trace. Wrongs on never-covered sub-concepts are lost.

**S1–S9 overall:** 142/161 correct (88%), 19 wrongs total — **only 7 traceable below**, 12 untraceable.

| Domain | Known wrongs | Untraceable wrongs total: 12 |
|---|---|---|
| Architecture | 3 (1.6 PUT/SnowSQL, 1.7 account-level objects, 1.9 Snowpark) | — |
| Governance | 1 (2.1 SECURITYADMIN vs USERADMIN) | — |
| Performance | 0 known | — |
| Data Loading | 2 (4.5 Root task RESUME, 4.6 Kafka connector) | — |
| Collaboration | 1 (5.3 replication edition) | — |
| **TOTAL TRACEABLE** | **7** | — |

**How to read this:** these are confusion points that historically tripped you up. Useful as a revision list, NOT as accuracy signal — denominators per domain are unknown.

### Topic Coverage

#### Architecture (103/117)
| Topic | Covered | Total | % |
|---|---|---|---|
| 1.1 Three-layer architecture ⭐ | 10 | 10 | 100% |
| 1.2 Virtual Warehouses ⭐ | 12 | 12 | 100% |
| 1.3 Micro-partitions ⭐ | 10 | 11 | 91% |
| 1.4 Data Clustering | 7 | 10 | 70% |
| 1.5 Snowflake editions ⭐ | 12 | 12 | 100% |
| 1.6 Snowflake interfaces | 7 | 9 | 78% |
| 1.7 Object hierarchy | 6 | 10 | 60% |
| 1.8 Table types | 8 | 10 | 80% |
| 1.9 AI/ML features | 7 | 8 | 88% |
| 1.10 Snowflake Cortex ⭐ | 8 | 8 | 100% |
| 1.11 Apache Iceberg tables | 8 | 9 | 89% |
| 1.12 Snowflake Notebooks ⭐ | 8 | 8 | 100% |

#### Governance (94/108)
| Topic | Covered | Total | % |
|---|---|---|---|
| 2.1 RBAC system roles ⭐ | 12 | 13 | 92% |
| 2.2 Role hierarchy ⭐ | 9 | 9 | 100% |
| 2.3 Authentication | 10 | 12 | 83% |
| 2.4 Network policies | 5 | 8 | 63% |
| 2.5 Dynamic Data Masking & RAP | 12 | 15 | 80% |
| 2.6 Column/row-level security ⭐ | 9 | 10 | 90% |
| 2.7 Encryption & Tri-Secret | 9 | 11 | 82% |
| 2.8 Cost management & monitors ⭐ | 11 | 11 | 100% |
| 2.9 Data lineage ⭐ | 8 | 8 | 100% |
| 2.10 Privacy policies ⭐ | 9 | 10 | 90% |

#### Performance (46/69)
| Topic | Covered | Total | % |
|---|---|---|---|
| 3.1 Query profile ⭐ | 11 | 11 | 100% |
| 3.2 Caching | 9 | 12 | 75% |
| 3.3 Warehouse tuning | 5 | 10 | 50% |
| 3.4 Clustering depth | 5 | 9 | 56% |
| 3.5 Search Optimization | 6 | 9 | 67% |
| 3.6 Materialized views | 6 | 9 | 67% |
| 3.7 Query Acceleration | 4 | 9 | 44% |

#### Data Loading (50/84)
| Topic | Covered | Total | % |
|---|---|---|---|
| 4.1 Stages | 7 | 11 | 64% |
| 4.2 COPY INTO | 9 | 13 | 69% |
| 4.3 File formats | 4 | 11 | 36% |
| 4.4 Snowpipe | 8 | 11 | 73% |
| 4.5 Streams and Tasks | 10 | 12 | 83% |
| 4.6 Connectors | 5 | 8 | 63% |
| 4.7 GET / PUT commands | 4 | 8 | 50% |
| 4.8 Unstructured data | 4 | 10 | 40% |

#### Collaboration (50/84)
| Topic | Covered | Total | % |
|---|---|---|---|
| 5.1 Secure Data Sharing ⭐ | 11 | 12 | 92% |
| 5.2 Snowflake Marketplace | 6 | 8 | 75% |
| 5.3 Data Replication | 6 | 10 | 60% |
| 5.4 Cloning | 4 | 10 | 40% |
| 5.5 Time Travel | 6 | 11 | 55% |
| 5.6 Fail-safe | 5 | 8 | 63% |
| 5.7 Data clean rooms | 5 | 8 | 63% |
| 5.8 Native apps | 4 | 9 | 44% |
| 5.9 Public vs private listings | 5 | 8 | 63% |

### Covered Sub-Concepts (audit trail)
- 1.1: Separation of storage and compute
- 1.2: Economy scaling waits ~6 min | Multi-cluster warehouses min/max
- 1.3: Micro-partitions are immutable
- 1.4: Large multi-TB tables with known filter columns benefit most
- 1.5: All editions include Fail-safe (7 days)
- 1.7: Warehouses are account-level objects
- 1.8: Transient persists across sessions; temporary does not
- 1.11: Iceberg interoperability — other engines can read same data
- 2.1: SECURITYADMIN — MANAGE GRANTS privilege
- 2.2: Privileges flow upward through role hierarchy
- 2.3: MFA enrolled per-user, enforceable by admin
- 2.4: Network policies control IP allowlist/denylist
- 2.5: Masking returns modified value; Row Access filters rows
- 2.7: Tri-Secret Secure: 3 keys total
- 2.8: SUSPEND vs SUSPEND_IMMEDIATE | Resource monitors can set any %
- 3.1: High partitions scanned vs total = pruning ineffective
- 3.2: Result cache 24h | Metadata queries need no warehouse
- ~~3.3: Scale out (multi-cluster) for high concurrency~~ (audited out — subsumed by later Scale UP/OUT bullet)
- 3.4: Lower clustering depth = better
- ~~3.5: SOS optimizes equality and IN predicates~~ (removed — Q12 wrong S14)
- 3.6: Materialized views auto-refreshed serverless
- 4.1: User stage (@~): auto-created per user
- 4.2: COPY INTO load history = 64 days | ON_ERROR controls behavior
- 4.4: Snowpipe event-driven via cloud notifications | Load history = 14 days
- 4.5: Root task must be RESUMED before children execute
- 4.6: Kafka connector uses Snowpipe internally
- 4.7: PUT only available in SnowSQL (CLI)
- 5.1: Reader accounts created by provider for non-Snowflake consumers
- 5.2: Marketplace = instant access, no ETL
- 5.3: Database replication = continuous sync across accounts
- 5.4: Zero-copy clone is metadata-only | Clone does NOT inherit privileges
- 5.5: Setting Time Travel retention to 0 disables it | UNDROP TABLE restores
- 5.6: Fail-safe = 7-day window, non-configurable
- 5.7: Clean rooms = secure multi-party data analysis
- 1.6: SnowSQL is the only interface supporting PUT/GET (not Snowsight, not drivers)
- 1.9: Snowpark = Python/Scala/Java for server-side data processing
- 1.12: Snowflake Notebooks = cell-based IDE in Snowsight (Python + SQL)
- 2.6: Tag-based masking policies apply masking via object tags
- 2.10: Aggregation policy prevents exposure of granular (individual-row) values
- 3.7: SYSTEM$ESTIMATE_QUERY_ACCELERATION('<query_id>') checks QAS eligibility; default scale factor = 8, 0 = unlimited
- 4.3: STRIP_OUTER_ARRAY = TRUE removes outer [ ] brackets when loading JSON arrays
- 4.8: Directory tables enable querying metadata for staged unstructured files
- 5.8: Native App logic (stored procs, functions) executes in consumer's account
- ~~1.1: Cloud Services layer = query optimization, metadata management, access control~~ (removed — Q3 wrong S14)
- 1.2: Auto-resume: warehouse resumes automatically on query submission if AUTO_RESUME = TRUE (default)
- 1.5: DDM requires Enterprise edition | Tri-Secret Secure requires Business Critical edition
- 1.8: Temporary table dropped at session end — no Time Travel recovery possible
- 1.9: Snowpark supports Python, Scala, and Java (languages — distinct from server-side sub-concept)
- 1.10: Cortex = suite of AI/LLM functions running natively in Snowflake without moving data
- 1.10: CORTEX.COMPLETE() is the function for LLM inference within Cortex
- 1.11: Iceberg external volume points to cloud object storage (S3, ADLS, GCS)
- ~~1.6: SnowSQL only for PUT~~ (removed — Q6 wrong, confused with Python connector)
- ~~1.7: Warehouses are account-level objects~~ (removed — Q16 wrong, missed Databases as account-level)
- ~~1.9: Snowpark = server-side processing without data movement~~ (removed — Q9 wrong)
- 1.6: PUT only available in SnowSQL — Snowsight, Python/JDBC/ODBC connectors do NOT support it (re-confirmed)
- 1.7: Account-level objects include Warehouses, Databases, Resource Monitors, Roles, and Users
- 2.1: SYSADMIN is the role for creating and managing data objects (databases, schemas, warehouses)
- 2.9: ACCESS_HISTORY tracks column-level access and data lineage (directSources, baseSources columns)
- 2.9: ACCESS_HISTORY lives in SNOWFLAKE.ACCOUNT_USAGE; ~3h latency, 365-day retention; requires Enterprise+
- 4.5: Insert-only streams are the only stream type supported on external tables
- 5.9: Private listing = shared with specific Snowflake accounts only; Public = visible to all Marketplace users
- 5.9: Marketplace listings deliver live read access — no data movement, no ETL (same as Secure Data Sharing)
- ~~2.1: SECURITYADMIN — MANAGE GRANTS privilege~~ (removed — Q8 wrong, confused with USERADMIN)
- ~~4.5: Root task must be RESUMED before children execute~~ (removed — Q9 wrong)
- 1.1: Cloud Services cost >10% of daily warehouse spend = extra credits billed
- 1.3: Micro-partitions store data in columnar compressed format
- 1.4: Automatic reclustering runs serverless in the background — no warehouse or manual steps
- 1.7: Named stages are schema-level objects
- 1.10: CORTEX.SUMMARIZE() generates text summaries; CORTEX.TRANSLATE() for translation
- 2.1: USERADMIN creates users; SYSADMIN creates data objects — distinct responsibilities
- 2.2: WITH GRANT OPTION lets a role pass received privileges downstream (vs MANAGE GRANTS = grant anything)
- 2.3: Key-pair authentication uses RSA public/private keys instead of passwords
- 2.4: User-level network policy overrides account-level network policy for that user
- 2.5: DDM and RAP are independent and stack — both apply simultaneously on the same table
- 2.5: DDM can be conditional — checks current role before deciding whether to mask
- 3.1: Spill to remote storage = memory and local disk exhausted — serious performance issue, fix with larger warehouse
- ~~3.2: COUNT(*)/MIN/MAX queries use metadata cache — no warehouse needed~~ (audited out — duplicate of "Metadata queries need no warehouse")
- ~~3.2: Result cache invalidated by: data change, 24h expiry, context (role) change; NOT affected by different warehouse~~ (removed — Q36 wrong S14)
- 3.2: Result cache is served by the Cloud Services layer — no virtual warehouse required to return a cached result (re-confirmed S18)
- 3.2: Result cache is account-wide — any user on any warehouse hits the same cached result if query + context match (re-confirmed S18)
- 3.3: Scale UP (larger warehouse) for slow individual queries; Scale OUT (multi-cluster) for concurrency
- 4.1: External stages reference cloud storage (S3, Azure Blob, GCS) for COPY INTO
- 4.2: SKIP_FILE = skips entire files with errors; CONTINUE = skips bad rows within files
- 4.8: Directory tables must be explicitly enabled on a stage to query file metadata
- ~~5.3: Secondary replica database is read-only; available cross-region and cross-cloud; all editions~~ (removed — CertSafari Q19 wrong; confused with failover)
- 5.3: Secondary replica database is directly queryable (read-only) WITHOUT failover — analysts just need USAGE privilege + a running warehouse in their account; failover only needed to promote secondary to primary for DR writes [CertSafari Q19 corrected]
- 1.9: Scalar UDF = returns one value per input row (Python/Java/Scala); UDTF = returns a table of rows; both run server-side in Snowflake [CertSafari Q10]
- 1.2: A SUSPENDED virtual warehouse consumes ZERO credits — credits only billed while warehouse is in RUNNING state [CertSafari Q38]
- 1.7: Parameter precedence: Session-level overrides User-level, which overrides Account-level — most specific setting wins [CertSafari Q26]
- 2.1: Object ownership (DAC): only the owner role can GRANT privileges on the object, DROP it, or TRANSFER ownership — even SYSADMIN cannot do these without taking ownership first [CertSafari Q36]
- 2.3: Snowflake ALERT = schema-level object evaluating a SQL condition on a schedule; when TRUE, fires an action (e.g. SYSTEM$SEND_EMAIL); used for data quality monitoring [CertSafari Q35]
- 3.2: Query Result Cache requires ALL: (1) underlying data unchanged, (2) exact query text match, (3) user has access privileges to all queried objects [CertSafari Q45]
- 3.5: "Search Optimization Access" node appears in Query Profile when a query successfully uses SOS — verify SOS impact via Query Profile [CertSafari Q24]
- 3.x: RANK() OVER (PARTITION BY col ORDER BY col DESC) = window function ranking rows within each partition; ties get same rank, next rank skips (1,1,3) [CertSafari Q15]
- 4.1: LIST @<stage_name> — SQL command to view all files currently in a Snowflake stage [CertSafari Q22]
- 4.3: FLATTEN() explodes nested arrays/objects in VARIANT columns into individual rows; use LATERAL FLATTEN(input => col:array) to unnest JSON arrays [CertSafari Q3]
- 4.3: SPLIT(string, delimiter) converts a delimited string into an ARRAY; combine with LATERAL FLATTEN to return each element as a separate row [CertSafari Q46]
- 4.5: Dynamic Tables refresh automatically and INCREMENTALLY — only processes changes since last refresh, not full table re-scans [CertSafari Q50]
- 5.2: Marketplace provider steps: create provider profile → build Share → create listing + attach share + add documentation/sample queries → publish [CertSafari Q49]
- 5.2: Marketplace consumers can submit dataset requests to providers through the Marketplace UI [CertSafari Q16]
- 1.11: Iceberg data files stored in Parquet format in customer-controlled cloud object storage (re-confirmed) [CertSafari Q7]
- 5.5: Transient tables have max 1-day Time Travel regardless of Snowflake edition
- ~~4.6: Kafka connector uses Snowpipe internally~~ (removed — Q22 wrong)
- ~~5.3: Database replication = continuous sync across accounts~~ (removed — Q28 wrong on edition)
- 4.6: Kafka Connector uses Snowpipe internally (re-confirmed S9 Q1)
- 4.6: Spark Connector integrates Spark DataFrames directly with Snowflake — no intermediate files
- 4.6: Python Connector executes SQL and fetches results — does NOT support PUT/GET commands
- 4.5: Standard streams on tables capture INSERT, UPDATE, and DELETE operations
- 4.5: Minimum Task schedule interval is ~10 seconds (not 1 minute — corrected per docs; old skill entry was outdated)
- 4.5: In a new Task DAG, each child task must be individually ALTERed to RESUME; shortcut: SYSTEM$TASK_DEPENDENTS_ENABLE(root_task_name) resumes the whole graph at once
- 4.5: Tasks are SUSPENDED by default on creation — must ALTER TASK ... RESUME before they run
- 5.1: Consumer in Secure Data Sharing needs their own virtual warehouse to query shared data (no data movement — reads provider's storage live)
- 5.3: Database replication (secondary replicas) is available on ALL Snowflake editions (Standard, Enterprise, BC, VPS)
- ~~2.1: SECURITYADMIN has the MANAGE GRANTS privilege — can grant any privilege on any object (re-confirmed S9 Q17)~~ (removed — Mock Exam R2 Q2 wrong; SYSADMIN vs SECURITYADMIN confusion persists)
- 3.4: average_overlap_depth ≈ 1.0 = micro-partitions are well-clustered with minimal overlap on the cluster key
- 3.5: SOS billed as serverless compute credits — separate from virtual warehouse credits
- 3.6: Materialized Views require Enterprise edition minimum
- 3.7: QAS benefits large analytical scans with selective filters, GROUP BY, ORDER BY — offloads to serverless compute
- 3.3: MAX_CONCURRENCY_LEVEL warehouse parameter controls max concurrent SQL statements before queuing begins
- 2.7: Snowflake encrypts data at rest using AES-256
- 2.10: Projection policy controls whether a column can be projected (returned) in SELECT query results
- 2.6: Row Access Policy condition can reference CURRENT_ROLE() or CURRENT_USER() to dynamically filter rows
- 5.6: Only Snowflake Support can initiate Fail-safe data recovery — customers cannot self-serve
- 5.6: Transient and Temporary tables have ZERO days of Fail-safe protection
- 5.7: Snowflake Clean Rooms are built on the Native App Framework — raw data never leaves the provider
- 5.8: Native Apps are distributed via the Snowflake Marketplace or private listings to consumers
- 1.9: ML.FORECAST is the Snowflake ML Function for time-series forecasting natively in Snowflake
- 1.12: Snowflake Notebooks support SQL, Python, and Markdown cells
- 4.3: INFER_SCHEMA automatically detects column names and data types from staged semi-structured/columnar files
- 4.7: GET command downloads files FROM a Snowflake stage TO the local filesystem (SnowSQL only)
- 4.3: MATCH_BY_COLUMN_NAME = CASE_INSENSITIVE maps file columns to table columns by name regardless of order
- 5.2: Data Exchange = private invitation-only data sharing hub (vs public Marketplace open to all Snowflake users)
- ⚠ CORRECTION: Periodic rekeying (re-encrypting data with new keys) = Enterprise+ feature; Business Critical adds Tri-Secret Secure (customer-managed key) — these are distinct
- 1.2: Auto-suspend default = 600 seconds (10 min); minimum = 60 seconds
- 1.3: Micro-partitions are 16–512 MB uncompressed (50–500 MB compressed)
- 1.4: SYSTEM$CLUSTERING_INFORMATION() returns clustering depth, overlap stats, partition counts
- 1.5: Multi-cluster warehouses, Row Access Policies, Time Travel (90 days) = Enterprise min; Fail-safe = ALL editions
- 1.6: Snowsight = browser-based web UI (SQL worksheets, query history, object explorer, dashboards); no installation needed
- 1.7: Database directly contains schemas (Org → Account → Database → Schema → Objects)
- 1.7: Schema-level objects include tables, views, stored procedures, stages, sequences, pipes, streams, tasks, functions
- 1.8: Temporary tables: no Fail-safe (0 days); no UNDROP after session ends; Time Travel available DURING the session
- 1.9: ML.ANOMALY_DETECTION = Snowflake ML Function for detecting anomalies in time-series data
- 2.3: SAML 2.0-based SSO = federated identity through an IdP (AD, Okta, Azure AD) for corporate login
- 2.3: OAuth 2.0 = delegated authorization; apps access Snowflake on behalf of a user without password sharing
- 2.7: Periodic rekeying = Enterprise+ minimum; Tri-Secret Secure = Business Critical minimum (distinct features)
- 2.8: Resource monitors can be assigned at account level or warehouse level (not database/schema level)
- 2.9: OBJECT_DEPENDENCIES view in SNOWFLAKE.ACCOUNT_USAGE tracks object-level dependency chains (view → table, etc.)
- 3.1: TableScan operator in Query Profile = reads data directly from storage micro-partitions
- 3.3: STATEMENT_QUEUED_TIMEOUT_IN_SECONDS = how long a queued statement waits before Snowflake returns an error
- 4.1: Table stage (@%table_name) is auto-created per table; can ONLY be used to load into that specific table
- 4.2: PURGE = TRUE removes source stage files after a successful COPY INTO load
- 4.4: S3 sends event notifications to SQS → Snowpipe polls SQS to trigger AUTO_INGEST
- 4.4: Recommended Snowpipe file size = 100–250 MB compressed
- 5.2: Snowflake Marketplace supports Native Applications as well as data listings
- 5.3: CREATE DATABASE <name> AS REPLICA OF <org>.<account>.<db> = creates a secondary replica database
- 5.4: Zero-copy clone shares storage initially; new writes to clone create new micro-partitions (billed separately)
- 5.1: External tables can be included in a data share and queried by consumers (read-only)
- 2.2: PUBLIC role is automatically granted to every user in Snowflake — no explicit grant needed
- 1.11: Snowflake-managed Iceberg tables: Snowflake manages the catalog internally — no external catalog (AWS Glue, etc.) required
- 3.6: Snowflake query optimizer can transparently rewrite queries to use a Materialized View — even when the base table is queried directly
- 4.8: GET_PRESIGNED_URL() generates a temporary, externally-accessible pre-signed URL for staged files — no Snowflake credentials needed; compare: BUILD_SCOPED_FILE_URL() (session token required), BUILD_STAGE_FILE_URL() (permanent, Snowflake auth required)
- 2.4: Network Rule is a schema-level object that defines IP address ranges (CIDR, host lists, private link IDs) — referenced by Network Policies
- 5.7: In a Snowflake Data Clean Room, data stays in each participant's own Snowflake account — only approved query results cross boundaries, not raw rows
- 3.4: High average_overlap_depth (e.g. 4.5) = poor clustering — many micro-partitions overlap on the key, pruning fails
- 2.1: ACCOUNTADMIN should be used sparingly — only for account-level tasks like billing and org settings
- 1.6: SnowSQL supports CLI scripting with variables and conditional logic (!if, !set) — suited for server-side automation
- 2.2: Custom roles should be granted to SYSADMIN so SYSADMIN can manage objects owned by those roles
- 1.12: Snowflake Notebooks support Git Integration — link to a Git repo in Snowsight for version control and sync
- 4.7: PUT command automatically compresses files with GZIP by default (disable with AUTO_COMPRESS = FALSE)
- 5.9: Snowflake Marketplace supports paid/monetized listings — providers set a price, Snowflake handles billing
- 3.4: Clustering keys provide minimal benefit on small tables — designed for multi-TB tables
- 2.2: ACCOUNTADMIN can view billing and credit usage — SYSADMIN cannot
- 5.8: Native Apps request specific privileges from consumer via setup script at install time — consumers grant/deny
- 3.5: SOS does NOT benefit full table scans (no WHERE clause) — designed for point lookups
- 2.4: Network policies can be applied at three levels: account, user, AND security integration
- 2.6: A masking policy function must return the SAME data type as the column it protects
- ~~1.3: Micro-partition metadata stores MIN, MAX, COUNT, DISTINCT COUNT per column — enables pruning and metadata-only queries~~ (removed — Q43 wrong S18; forgot DISTINCT COUNT)
- 2.1: USERADMIN creates users and roles but CANNOT grant privileges — SECURITYADMIN holds MANAGE GRANTS
- 1.4: CLUSTER BY (col) clause defines a clustering key when creating a Snowflake table
- 1.2: Warehouse credits billed per-second with a 60-second minimum billing period at startup
- 3.7: QAS offloads eligible SELECT query processing to serverless compute — NOT additional warehouse clusters
- 4.4: Snowpipe triggered via AUTO_INGEST (cloud event notifications) OR REST API calls
- 1.9: Cortex AI = LLM-based functions (COMPLETE, SUMMARIZE, TRANSLATE, SENTIMENT); Snowpark ML = traditional ML (scikit-learn, forecasting)
- 5.4: Cloning a database cascades to all child schemas, tables, and objects — cloned atomically and instantaneously
- 5.5: Time Travel AT/BEFORE supports three options: TIMESTAMP, OFFSET (seconds ago), STATEMENT (query ID)
- 3.3: STATEMENT_TIMEOUT_IN_SECONDS cancels running queries; STATEMENT_QUEUED_TIMEOUT_IN_SECONDS cancels queries waiting in queue
- 2.9: ACCESS_HISTORY directSources = immediate upstream column; baseSources = original source through all transformations
- 4.2: VALIDATION_MODE = 'RETURN_ERRORS' returns errors in staged files WITHOUT loading any data — dry run
- 3.1: Aggregate node in Query Profile performs GROUP BY and aggregation operations
- 4.1: Named internal stages are schema-level objects usable with any table; table stages auto-created and single-table only
- 2.7: Snowflake hierarchical encryption: account master key → table master key → file key
- 4.3: Semi-structured data (JSON, Parquet, Avro, ORC, XML) loaded into VARIANT columns
- 1.8: Default table type is permanent (full Time Travel + Fail-safe) when no type specified in CREATE TABLE
- 2.8: Resource monitor NOTIFY = alert only, queries continue; SUSPEND = waits for current queries then suspends
- 5.2: Trial listings on Marketplace allow consumers to access a data subset free before committing to paid
- 4.5: SYSTEM$STREAM_HAS_DATA('stream_name') returns TRUE if stream has unconsumed records — used in Task WHEN clause
- 1.7: Sequences are schema-level objects (along with tables, views, pipes, streams, tasks, stages, functions)
- 3.2: Local disk cache lives in warehouse SSD — lost when warehouse suspends; each warehouse has its own
- 4.6: Kafka Connector uses Snowpipe (serverless) internally — billed as serverless compute credits, not warehouse credits
- 1.10: CORTEX.SENTIMENT() analyzes text for positive/negative/neutral emotional tone
- 3.6: Snowflake Materialized Views cannot include JOINs across multiple base tables — limited to single base table
- 5.3: Secondary replica databases require a REFRESH operation (manual or scheduled) — NOT real-time sync
- 1.11: Catalog Integration = Snowflake object connecting to external Iceberg catalogs (AWS Glue, Apache Polaris) to query external Iceberg tables
- 1.5: VPS (Virtual Private Snowflake) = completely isolated — dedicated compute, storage, AND Cloud Services/metadata layer
- 1.4: Clustering keys support deterministic expressions (e.g., TO_DATE(event_time)) — not limited to raw column references
- 1.3: Without a clustering key, data loads in insertion order — micro-partitions overlap on all columns, pruning fails for equality filters
- 1.1: Multiple virtual warehouses run concurrently against the same Storage layer — no data duplication required
- 1.2: Warehouse credit consumption doubles per size step: XS=1, S=2, M=4, L=8, XL=16, 2XL=32, 3XL=64, 4XL=128 credits/hour
- 3.1: HashJoin node in Query Profile = most common join type; expensive when both sides are large and unfiltered — fix with selective pre-filters
- 3.6: Materialized Views cannot include non-deterministic functions (CURRENT_DATE(), CURRENT_TIMESTAMP(), RANDOM())
- 5.9: Public Marketplace listings are accessible cross-cloud and cross-region — Snowflake auto-replicates behind the scenes; consumer queries it as a normal database
- 5.8: Application Package = provider-side container holding app definition, versioned releases, and setup scripts for Native Apps
- 5.5: DATA_RETENTION_TIME_IN_DAYS inheritance — table inherits from schema if unset; schema from database; most specific setting wins
- 5.6: Fail-safe period begins immediately after Time Travel retention ends — dropped table recoverable for Time Travel + 7 more days (Snowflake Support only)
- 4.2: COPY INTO PATTERN option accepts a regex string to load only files matching the pattern from a stage
- 1.1: Cloud Services layer manages transactions — ACID compliance and concurrency control
- 1.1: Storage layer stores data in columnar compressed format as Snowflake-managed micro-partitions
- 2.3: SCIM automatically provisions and deprovisions users and groups from an IdP into Snowflake
- 2.5: USING clause in a DDM policy passes additional column values as context for conditional masking logic
- 2.7: Revoking the customer KMS key in Tri-Secret Secure makes all data immediately inaccessible — all three keys required for decryption
- 2.8: SUSPEND_IMMEDIATE kills all running queries immediately and suspends the warehouse (SUSPEND waits for running queries to finish)
- 3.2: When local SSD is exhausted, Snowflake spills intermediate results to remote cloud object storage (S3/Azure Blob/GCS)
- ~~3.5: ALTER TABLE ... ADD SEARCH OPTIMIZATION — correct syntax to enable SOS on a table (not SET, not ENABLE)~~ (removed — Q40 wrong S18; picked ENABLE)
- 3.5: Search Optimization Service requires Enterprise edition minimum
- ~~3.7: QAS only accelerates SELECT queries — DML statements (UPDATE, INSERT, DELETE) are not eligible~~ (removed — Q35 wrong S18; also picked INSERT…SELECT as eligible)
- 5.1: Consumer must grant IMPORTED PRIVILEGES ON DATABASE <shared_db> TO ROLE <role> before querying shared data
- 5.1: Only SECURE VIEWs can be included in a data share — regular views cannot be shared
- ~~2.10: Projection policy returns NULL for blocked columns~~ (removed — Q18 S15 wrong; confusion with excluded vs NULL persists)
- 4.5: METADATA$ACTION column in streams indicates the DML operation type (INSERT or DELETE; UPDATE = DELETE + INSERT pair)
- 3.1: QUERY_HISTORY view in SNOWFLAKE.ACCOUNT_USAGE provides historical query performance data across the entire account
- 4.4: Snowpipe Streaming billed in compute-seconds (distinct from regular Snowpipe serverless file credits)
- 4.5: Dynamic Tables = declarative pipeline approach; specify target SQL, Snowflake auto-manages refresh (vs manual Streams + Tasks)
- 5.3: Failover operation promotes a secondary database replica to primary — allows writes on the replica during DR
- 5.2: ACCOUNTADMIN has default privileges to create and manage Marketplace listings
- 1.2: For infrequent batch jobs (e.g. 8 min/hour), optimal AUTO_SUSPEND = 60s (minimum) to avoid paying for idle time
- 2.1: Discretionary Access Control (DAC) = object owners decide who can access their objects via GRANT
- 2.8: WAREHOUSE_METERING_HISTORY view (ACCOUNT_USAGE) tracks compute credits consumed per warehouse over time
- 3.1: Exploding/Cartesian joins result from non-equality or missing join conditions — massive row multiplication
- 4.1: STORAGE INTEGRATION eliminates embedding credentials in SQL/stages — centralized, secure cloud storage access
- ~~5.5: Transient tables have max 1-day Time Travel regardless of Snowflake edition~~ (removed — CertSafari Q18 wrong; confused with External tables which have NO Time Travel)
- 1.9: Snowflake ML components: Feature Store (feature engineering), Modeling API (training), Model Registry (versioning/deployment)
- 1.8: External Tables = read-only tables querying data directly in external cloud storage (S3/Azure/GCS) without loading into Snowflake
- 2.1: Snowflake RBAC core model — privileges are granted to roles; roles are granted to users; privileges are NEVER granted directly to users
- 2.2: RBAC best practice — create a named role (e.g. MARKETING_ANALYST), grant all required object privileges to the role, then grant the role to the user; avoids privilege sprawl
- 2.7: Snowflake does NOT provide user-level encryption keys — the encryption hierarchy is account master key → table master key → file key only
- 2.9: ACCOUNT_USAGE schema views retain historical data for up to 365 days (1 year) — e.g. QUERY_HISTORY, WAREHOUSE_METERING_HISTORY, ACCESS_HISTORY all have 365-day lookback
- 2.9: The SNOWFLAKE shared database (which contains ACCOUNT_USAGE schema) is read-only and automatically available in every Snowflake account — no explicit sharing or setup required
- 2.8: Warehouse-level resource monitors only affect the assigned warehouse — a warehouse with NO resource monitor continues running unaffected even when another warehouse's RM triggers a Suspend action
- 2.9: Data lineage (conceptual): tracks the full movement and transformation of data from its original source(s) through all intermediary steps to its final destination
- 2.9: Querying SNOWFLAKE.ACCOUNT_USAGE views requires ACCOUNTADMIN by default; lower-privilege roles can access via SNOWFLAKE database roles (OBJECT_VIEWER, USAGE_VIEWER, GOVERNANCE_VIEWER)
- 2.2: GRANT ROLE <child_role> TO ROLE <parent_role> — establishes role hierarchy so child_role inherits all privileges held by parent_role; privileges flow upward through the hierarchy
- 1.7: Snowflake preferred account identifier: <organization_name>-<account_name> — globally unique, human-readable; preferred over the legacy account_locator.region.cloud format
- 1.3: DML changes (INSERT/UPDATE/DELETE) in Snowflake create new micro-partitions and retire old ones — immutability is what enables Time Travel (old partitions kept) and Fail-safe to function
- 1.5: Standard edition: Time Travel retention max = 0 or 1 day; Enterprise edition+ allows up to 90 days for permanent tables
- 1.10: Cortex Analyst = natural language (conversational) interface for querying structured data in specific Snowflake tables; translates business questions into SQL automatically — distinct from Cortex Search which handles unstructured content
- 1.2: CREATE WAREHOUSE <name> [WITH WAREHOUSE_SIZE = 'X-SMALL'] is the DDL to create a virtual warehouse — default size is X-SMALL if omitted
- 1.6: ODBC driver enables BI tools (Tableau, Power BI) and ETL tools to connect to Snowflake via the ODBC standard — not language-specific, unlike language connectors (Python, JDBC, .NET)
- 1.7: Sequences generate unique, sequential numbers; referenced in SQL via <seq_name>.NEXTVAL — used for primary keys when table has no IDENTITY column
- 2.6: Context Functions (CURRENT_USER(), CURRENT_ROLE(), CURRENT_DATABASE(), etc.) return the active session context — commonly referenced in Row Access Policies and masking conditions for dynamic filtering
- 2.7: Internal stage files (files uploaded via PUT) are encrypted with a Snowflake-managed key using AES-128 or AES-256 depending on the stage configuration
- 2.8: QUERY_HISTORY (SNOWFLAKE.ACCOUNT_USAGE) records all executed SQL — DDL, DML, and queries — use it to audit who ran DROP TABLE, not just for query performance analysis
- 4.2: ON_ERROR default in COPY INTO = ABORT_STATEMENT — aborts the entire load statement and rolls back on the first file with errors; no rows from any file are loaded
- 4.2: COPY INTO @<stage_name> FROM <table> is the unloading syntax — same COPY INTO command but target is a stage, source is a table (reverse of loading direction)
- 5.1: CREATE DATABASE <db_name> FROM SHARE <provider_org>.<provider_account>.<share_name> creates the consumer's local database object from an inbound share
- 5.1: ALTER SHARE <share_name> ADD ACCOUNTS = <account_id> adds a consumer account to a share without replacing existing consumers (SET ACCOUNTS would replace the full list)
- 5.1: Direct Share = provider shares data directly with named consumer accounts (via ACCOUNTS clause on ALTER SHARE) — no Marketplace listing needed; consumer accounts are explicitly specified
- ~~3.7: ALTER WAREHOUSE <wh> SET ENABLE_QUERY_ACCELERATION = TRUE enables QAS on a specific warehouse; QUERY_ACCELERATION_MAX_SCALE_FACTOR sets the max serverless resource multiplier~~ (removed — Q41 wrong S18; picked query-level hint)
- 2.6: Object tags can be applied to virtually any Snowflake securable object — databases, schemas, tables, columns, views, warehouses, users, roles, and more
- 3.3: Workload isolation pattern: separate warehouses for ETL vs BI workloads eliminates query queuing contention — each team scales independently with no interference
- 5.7: Clean room overlap analysis: INNER JOIN on a hashed/pseudonymized column (e.g., hashed email) + COUNT(DISTINCT) = industry-standard technique to measure shared audience without exposing any raw PII rows
- 3.5: SOS billing has two separate cost components: (1) storage cost for the search access path (extra data structures maintained on disk) + (2) serverless compute credits to build and continuously maintain that path
- 2.8: Object tags used for cost allocation: tag a warehouse or table with a cost center value → query SNOWFLAKE.ACCOUNT_USAGE.TAG_REFERENCES to allocate credit usage by business unit
- 2.8: Resource monitor configurable properties: CREDIT_QUOTA (number of credits before trigger), FREQUENCY (reset period: DAILY/WEEKLY/MONTHLY/YEARLY/NEVER), START_TIMESTAMP (when monitoring begins), and threshold-based actions (NOTIFY/SUSPEND/SUSPEND_IMMEDIATE at specified % of quota)
- 2.2: USE ROLE <role_name> switches the active role for the current session only — does NOT change the user's DEFAULT_ROLE; effect ends when session ends or USE ROLE is called again
- 2.10: MIN_GROUP_SIZE on an aggregation policy: groups below the threshold are suppressed entirely from query results (not replaced with NULL — just absent from output) [S16 Gov Drill]
- 2.5: Row Access Policy applied with: ALTER TABLE t ADD ROW ACCESS POLICY p ON (col_list) — ADD not SET; ON clause specifies which columns enforce the filter [S16 Gov Drill]
- 2.5: RAP is a schema-level object — must be created in a schema; referenced by tables/views using ALTER TABLE [S16 Gov Drill]
- 2.1: ORGADMIN role manages organization-level features — creates new Snowflake accounts, views org-wide usage, enables cross-account replication and failover; does NOT manage within-account object privileges [S16 Gov Drill]
- 2.4: ALLOWED_IP_LIST = explicit IP whitelist on a network policy; any IP not listed is blocked from connecting to Snowflake [S16 Gov Drill]
- 2.3: Password Policy = Snowflake schema-level object defining password complexity/expiry rules; applied via ALTER ACCOUNT SET PASSWORD POLICY or ALTER USER SET PASSWORD POLICY [S16 Gov Drill]
- 2.10: Projection policy NULLIFY mode: WHERE clause evaluates real column values; SELECT output returns NULL for the restricted column (re-added after S15 removal) [S16 R2]
- 2.1: SECURITYADMIN holds the MANAGE GRANTS privilege — can grant any privilege on any object in the account (re-added after Mock Exam R2 removal) [S16 R2]
- 2.3: ALTER USER <name> SET RSA_PUBLIC_KEY = '<public_key>' configures key-pair authentication on a Snowflake user; private key stays on client, never sent to Snowflake [S16 R2]
- 2.4: BLOCKED_IP_LIST on a network policy overrides ALLOWED_IP_LIST — an IP in both lists is denied [S16 R2]
- 2.10: Aggregation policy is applied at the table or view level — not at column level [S16 R2]
- 2.6: APPLY privilege on the masking policy is required to attach it to a table column (separate from CREATE MASKING POLICY) [S16 R2]
- 2.1: Managed Access Schema — schema owner centralizes all privilege grants; object owners cannot directly GRANT privileges on their own objects [S16 R2]
- 2.10: Projection policy FAIL mode: if a query references the restricted column, the entire query errors out — stricter than NULLIFY which returns NULL [S16 R2]
- ~~2.5: ALTER TABLE t ALTER COLUMN col SET MASKING POLICY p — correct DDM attachment syntax; ALTER TABLE → ALTER COLUMN → SET MASKING POLICY [S17]~~ (removed — Q8 wrong S18; picked SET…ON COLUMN)
- 2.7: Snowflake encrypts data in transit using TLS 1.2 or higher (not SSL, not TLS 1.0) [S17]
- 2.5: EXEMPT MASKING POLICY privilege allows a role to bypass ALL Dynamic Data Masking policies and see unmasked data — account-level privilege, only granted to data stewards [S17]
- 2.5: Only ONE masking policy can be applied to a single column at a time — conditional logic must be built inside the single policy function [S17]
- 2.2: USERADMIN is a child of SECURITYADMIN in the default Snowflake role hierarchy (ACCOUNTADMIN → SECURITYADMIN → USERADMIN) [S17]
- 2.3: Authentication Policy = Snowflake schema-level object that enforces which authentication methods (MFA, SSO, password) are allowed for users or the account [S17]
- 2.5: Dynamic Data Masking masks values in WHERE clause predicates too — not just SELECT output; prevents inference attacks (contrast: Projection Policy NULLIFY allows WHERE to use real values) [S17]
- 2.6: Tag inheritance/propagation — when a tag is applied to a parent object (e.g., schema), it propagates to all child objects (tables, columns) automatically; child objects can override the inherited value [S17]
- 2.5: Only ONE Row Access Policy can be applied to a table at a time — to swap, DROP the existing policy first, then ADD the new one [S17]
- 2.10: APPLY privilege on a projection policy is required to attach it to a table or view (same pattern as APPLY on a masking policy) [S17]
- 2.6: Database roles are scoped to a single database — privileges apply only within that database; can be granted to account roles/users but cannot reach objects in other databases [S17]
- 2.1: ACCOUNTADMIN best practice — grant to as few users as possible, ideally 2–3 named individuals for redundancy; never share credentials or grant broadly [S17]
- 2.10: Aggregation policies and projection policies are schema-level objects — created inside a schema (same as masking policies, RAPs, password policies, authentication policies) [S17]
- 2.3: External OAuth role mapping — Snowflake reads claims in the OAuth token (e.g., role/group membership) to determine which Snowflake role to activate for the session [S17]
- ~~2.3: In SAML 2.0 SSO flow, the Identity Provider (IdP) — e.g., Okta, Azure AD, ADFS — issues the SAML assertion; Snowflake (Service Provider) validates and accepts it [S17]~~ (removed — Q1 wrong S18; SAML/OAuth confusion 4th instance)
- 2.3: SAML assertion = XML-based document digitally signed by the IdP; OAuth access tokens = JWT/opaque strings (distinct sub-concept re-confirmed S18)
- ~~2.3: SAML 2.0-based SSO = federated identity through an IdP (AD, Okta, Azure AD) for corporate login~~ (removed — Q3 wrong S17; confused SAML assertion with OAuth token; partial recovery via Q30 IdP sub-concept)
- 1.1: Cloud Services layer = query optimization, metadata management, authentication, and access control (re-confirmed CS-May30 Q36; re-added after S14 removal)
- 1.2: Snowpark-optimized warehouse has significantly more memory per node — designed for memory-intensive Snowpark ML workloads (model training, feature engineering) [CS-May30 Q30]
- 1.2: ALTER WAREHOUSE <name> SET WAREHOUSE_SIZE = '<size>' — DDL to dynamically resize an existing warehouse [CS-May30 Q39]
- 3.1: RESULT_SCAN(LAST_QUERY_ID()) = table function that returns the result set of a previous query; enables querying prior results without re-executing the query [CS-May30 Q3]
- 3.1: CTE (Common Table Expression) using WITH clause — names intermediate result sets for use later in the same query; ideal for multi-step aggregation or readability [CS-May30 Q14]
- 3.1: GROUP BY + HAVING for aggregate filtering — HAVING applies AFTER aggregation (filters groups); WHERE applies BEFORE (filters rows); use HAVING to filter on aggregate functions like AVG(), COUNT() [CS-May30 Q41]
- 3.2: ALTER SESSION SET USE_CACHED_RESULT = FALSE — disables Query Result Cache for the current session, forcing fresh execution [CS-May30 Q38]
- 4.6: .NET, Go, and Node.js are among Snowflake's native language connectors (alongside Python, JDBC, ODBC, Spark, Kafka) [CS-May30 Q20]
- 5.1: Resharing = a consumer who has been granted explicit permission by the provider can create a new share containing the provider's data and share it onward with a third account [CS-May30 Q8]
- 5.2: Free Marketplace listing billing: consumers pay zero for the data itself but pay their own standard compute costs to query it [CS-May30 Q45]
- 5.4: Zero-copy clone of a table also copies Time Travel data (historical micro-partition versions) AND any data masking policies applied to the table [CS-May30 Q37]
- 1.8: Hybrid Tables (HTAP) = Snowflake table type supporting ACID transactions (row-based storage) AND analytical queries (columnar storage) in the same table — designed for mixed OLTP/OLAP without dual systems [Arch Drill Q1]
- 1.12: Notebooks use waterfall execution — cells run top-to-bottom; each cell's output is available to all subsequent cells; must run earlier cells before later ones can use their results [Arch Drill Q2]
- 1.5: Database Failover/Failback = Business Critical edition minimum; Failover promotes a secondary replica to primary for disaster recovery writes [Arch Drill Q4]
- 1.6: Snowflake Extension for VS Code = IDE plugin providing SQL authoring, object explorer, and query execution inside VS Code — distinct from SnowSQL (standalone CLI tool) [Arch Drill Q5]
- 1.4: CLUSTER BY (col1, col2) — multi-column clustering key; data sorted primarily by col1, then col2; can be defined at CREATE TABLE or added via ALTER TABLE CLUSTER BY [Arch Drill Q6]
- 1.11: External Volume is required for BOTH Snowflake-managed AND externally-managed Iceberg tables — provides the cloud object storage connection (S3/ADLS/GCS) where Iceberg data files physically live [Arch Drill Q7]
- 1.11: Catalog Integration is required ONLY for externally-managed Iceberg tables (AWS Glue, Apache Polaris) — Snowflake-managed Iceberg tables do NOT need a Catalog Integration [Arch Drill Q7]
- 1.5: HIPAA and PCI-DSS compliance = Business Critical edition minimum — required for healthcare and payment card data regulatory requirements [Arch Drill Q8]
- 1.12: Snowflake Notebooks can use a Snowpark-optimized warehouse (provides more memory per node) for ML/data science workloads — selected at the notebook level [Arch Drill Q9]
- 1.1: The Storage layer uses object storage infrastructure from the underlying cloud provider (AWS S3, Azure Blob Storage, or GCS) — Snowflake manages data organization on top of cloud-provider storage [Arch Drill Q10]
- 1.9: Document AI = Snowflake feature using foundation models to extract structured information from unstructured documents (PDFs, images) — returns key-value pairs from document content [Arch Drill Q12]
- 1.10: CORTEX.EXTRACT_ANSWER(document_text, question) = Cortex function that reads a document and returns a direct answer to a specific question — designed for Q&A retrieval from long-form text [Arch Drill Q13]
- 1.12: Snowflake Notebooks can be scheduled to run automatically by linking them to Snowflake Tasks — enables periodic notebook execution (e.g., nightly data refresh) without manual triggers [Arch Drill Q14]
- 1.8: Event Tables = special Snowflake table type for storing telemetry data (logs, traces, metrics) from Snowflake-hosted code (UDFs, stored procedures) and external systems — purpose-built for observability [Arch Drill Q15]
- 1.5: Search Optimization Service (SOS) = Enterprise edition minimum — NOT available on Standard edition [Arch Drill Q18]
- 1.3: APPROX_COUNT_DISTINCT() can leverage HyperLogLog (HLL) sketches stored in micro-partition metadata — avoids full data scan; exact COUNT(DISTINCT) cannot use HLL sketches and must scan raw data [Arch Drill Q19]
- 1.10: Cortex Search = Snowflake's semantic/vector search service for unstructured content — indexes documents and answers NL queries by finding relevant passages; distinct from Cortex Analyst (NL→SQL for structured tables) [Arch Drill Q21]
- 1.5: Periodic rekeying = Enterprise edition minimum; automatically re-encrypts data with a new AES key on a schedule — distinct from Tri-Secret Secure (BC edition, customer-managed key in their KMS) [Arch Drill Q22]
- 1.9: ML MODEL = schema-level Snowflake object (stored in a schema alongside tables, views, functions, stages) — NOT an account-level object [Arch Drill Q23]
- 1.11: CREATE ICEBERG TABLE <name> CATALOG = 'SNOWFLAKE' EXTERNAL_VOLUME = '<vol_name>' BASE_LOCATION = '<path/>' — DDL for a Snowflake-managed Iceberg table; CATALOG='SNOWFLAKE' means Snowflake owns and manages the catalog [Arch Drill Q24]
- 1.1: Cloud Services layer accrues compute credits even when NO virtual warehouses are running — billed as additional charge only when CS costs exceed 10% of that day's total warehouse compute spend [Arch Drill Q26]
- 1.12: Snowflake Notebooks support Anaconda package installation — the Anaconda curated channel provides Python packages (NumPy, pandas, scikit-learn, etc.) pre-validated for Snowflake environments [Arch Drill Q27]
- 1.5: Column-level Security (column masking policies) = Enterprise edition minimum [Arch Drill Q28]
- 1.9: Cortex Fine-tuning = Snowflake feature to fine-tune a foundation LLM (Mistral, Llama) on customer data in a Snowflake table — produces a private customized model version stored in the account [Arch Drill Q29]
- 1.12: Snowflake Notebooks natively support Streamlit — Python cells can use st.slider, st.selectbox, st.write, etc. for interactive UI elements directly inside the notebook without a separate deployment [Arch Drill Q30]
- 1.3: Micro-partition metadata stores NULL count per column (alongside min/max, distinct count) — enables NULL-aware pruning [Q9]
- 1.6: Snowsight Data Preview and Column Statistics — click any table in the object explorer to see row count, column types, and distribution stats at a glance without writing SQL [Q33]
- ~~1.4: CLUSTER BY (col) clause defines a clustering key when creating a Snowflake table~~ (removed — Q17 wrong; confused CLUSTER ON for CLUSTER BY; re-adding below)
- 1.4: CLUSTER BY (col) clause is the correct DDL syntax for defining a clustering key; CLUSTER ON and PARTITION BY are not valid Snowflake syntax [Q17 re-confirmed]
- 2.1: To query any Snowflake object, a role needs USAGE on the parent database AND parent schema PLUS the object-level privilege (e.g. SELECT) — missing USAGE on db or schema causes 'object does not exist or not authorized' [Q46]
- 2.8: QUERY_TAG session parameter (ALTER SESSION SET QUERY_TAG = 'dept:finance') tags queries for cost attribution — filter in QUERY_HISTORY by QUERY_TAG to allocate costs by department or project [Q37]
- ~~3.3: MAX_CONCURRENCY_LEVEL warehouse parameter controls max concurrent SQL statements before queuing begins~~ (removed — Q12 wrong; confused with AUTO_SUSPEND; re-adding below)
- 3.3: MAX_CONCURRENCY_LEVEL controls the max concurrent SQL statements before queuing begins — directly manages queue behavior; AUTO_SUSPEND has nothing to do with queuing [Q12 re-confirmed]
- 3.1: QUERY_HISTORY.EXECUTION_STATUS = 'FAILED' and ERROR_CODE columns identify failed queries — use these two columns together to find queries that errored with specific error codes [Q41]
- 3.2: Non-deterministic functions (CURRENT_TIMESTAMP(), CURRENT_DATE(), SYSDATE(), RANDOM()) prevent Query Result Cache reuse — query re-executes fresh every time even if all other conditions match [Q25]
- 3.2: DESCRIBE TABLE <name> uses the metadata cache — returns schema instantly with no running warehouse required (same principle as COUNT(*)/MIN/MAX metadata-only queries) [Q5]
- 4.1: Storage Integration supports exactly three cloud providers: Amazon S3, Microsoft Azure Blob Storage, and Google Cloud Storage — NOT consumer/personal cloud storage (Dropbox, Drive, iCloud) [Q11]
- 4.2: COPY_HISTORY view in SNOWFLAKE.ACCOUNT_USAGE tracks COPY INTO load jobs with 365-day history; LOAD_HISTORY is the equivalent in INFORMATION_SCHEMA with only 14-day history — both are queryable for COPY INTO auditing [Q2 — missed this, selected DATA_TRANSFER_HISTORY]
- 4.3: PARSE_JSON(<string>) converts a JSON-formatted VARCHAR string into a VARIANT type — the inverse of TO_JSON() [Q50]
- 4.4: Snowpipe Streaming offsetToken — the SDK client passes a string token marking its last processed record; on crash/restart, the client resumes from the last committed offset to prevent duplicate ingestion [Q20]
- 4.8: Directory table columns include RELATIVE_PATH, FILE_URL, FILE_SIZE, LAST_MODIFIED, STAGE_NAME, MD5 — ROW_COUNT is NOT a column (files don't have row counts until loaded) [Q21 — missed STAGE_NAME, wrongly picked ROW_COUNT]
- 5.1: Virtual warehouses cannot be included in a data share — only data objects (tables, views, schemas, databases) can be shared; consumers always use their OWN warehouse to query shared data [Q10]
- 5.1: Shared database queried using standard 3-part notation: SELECT * FROM shared_db.schema.table — no provider prefix needed in the query; the CREATE DATABASE FROM SHARE already establishes the link [Q7 — missed this, used bare table name without db.schema prefix]
- 5.5: Time Travel restore: (1) CREATE OR REPLACE TABLE t CLONE t AT(TIMESTAMP => <ts>) restores table in-place; (2) CREATE TABLE t_restore AS SELECT * FROM t AT(TIMESTAMP => <ts>) reconstructs from historical data — both are valid restore patterns [Q30]

---

## Sessions (delta log — most recent first)

### External Practice — 2026-05-31 (50 questions, mixed domains)
- Score: 45/50 (90%)
- Source: External practice exam (no XP awarded)
- New sub-concepts: +12 covered, -2 removed, +3 uncovered = **+10 net covered** (313 → 323 / 447 → 462)
- Removed: ~~1.4 CLUSTER BY syntax~~ (Q17 wrong — confused CLUSTER ON vs CLUSTER BY) | ~~3.3 MAX_CONCURRENCY_LEVEL~~ (Q12 wrong — confused with AUTO_SUSPEND)
- New covered: 1.3 NULL count in micro-partition metadata | 1.4 CLUSTER BY re-confirmed | 1.6 Snowsight Data Preview | 2.1 USAGE on DB+schema | 2.8 QUERY_TAG | 3.1 ERROR_CODE/EXECUTION_STATUS | 3.2 non-deterministic functions prevent cache | 3.2 DESCRIBE TABLE = metadata cache | 3.3 MAX_CONCURRENCY_LEVEL re-confirmed | 4.1 Storage Integration providers | 4.3 PARSE_JSON | 4.4 offsetToken | 5.1 VWH not shareable | 5.5 TT restore CLONE AT + CTAS AT
- New uncovered: 4.2 COPY_HISTORY (ACCOUNT_USAGE) | 5.1 3-part notation for querying shared DB | 4.8 STAGE_NAME in directory table (not ROW_COUNT)
- Wrong answers: Q2 (missed COPY_HISTORY — picked DATA_TRANSFER_HISTORY) | Q7 (3-part notation for shared DB — picked bare table name) | Q12 (MAX_CONCURRENCY_LEVEL — picked AUTO_SUSPEND) | Q17 (CLUSTER BY syntax — picked CLUSTER ON) | Q21 (STAGE_NAME in dir table — picked ROW_COUNT)
- Per-domain accuracy this session: Arch 12/13 (92%) | Gov 8/8 (100%) | Perf 8/9 (89%) | Load 9/11 (82%) | Collab 8/9 (89%)
- ⚠️ 5.1 Secure Data Sharing LOSES mastery star: was 9/10=90% ⭐, now 10/12=83% (2 new pool items from this session)
- Updated accuracy: Arch 132/154 (86%) | Gov 149/187 (80%) | Perf 71/83 (86%) | Load 61/68 (90%) | Collab 72/81 (89%) | Total 485/573 (85%)
- Gov accuracy crosses 80% mark! Final Boss still locked (79.7% — 0.3% below threshold)
- Domain mastery: Arch 92→93/115→117 (80%→79%) | Gov 87→89/106→108 (82%) | Perf 40→42/66→69 (61%) | Load 44→47/79→84 (56%) | Collab 47→49/81→84 (58%)
- Persistent confusion: CLUSTER BY vs CLUSTER ON (syntax!), 3-part query notation for shares, COPY_HISTORY vs LOAD_HISTORY distinction
- Questions: 710→**760** | Sub-concepts: 313/447→**323/462 (69.9%)** | XP: unchanged (9973) | Exam date: unchanged (June 8 ✅)

### Architecture Drill — 2026-05-30 (30 questions, Architecture domain focus)
- Score: 27/30 (90%) — Q11 voided (disputed: exact vs approx distinct count in micro-partition metadata; full credit given); Q17/Q20/Q25 wrong
- XP delta: +635 XP (27 correct × 20 XP + 95 streak bonus — streak ran Q1–Q16 = 16 consecutive incl. void)
- Best streak this session: 16 (Q1–Q16, Q11 void maintained streak) | All-time best: 22 (unchanged)
- New sub-concepts: **+25 net** (no removals — all wrong answers hit uncovered sub-concepts)
- Added: 1.8 Hybrid Tables/HTAP | 1.12 waterfall execution | 1.5 Failover/Failback=BC | 1.6 VS Code Extension | 1.4 CLUSTER BY multi-col | 1.11 External Volume (both types) | 1.11 Catalog Integration (external only) | 1.5 HIPAA/PCI=BC | 1.12 Snowpark-optimized WH for Notebooks | 1.1 cloud provider object storage | 1.9 Document AI | 1.10 EXTRACT_ANSWER | 1.12 Tasks scheduling for Notebooks | 1.8 Event Tables | 1.5 SOS=Enterprise | 1.3 APPROX_COUNT_DISTINCT HLL | 1.10 Cortex Search | 1.5 Periodic rekeying=Enterprise | 1.9 MODEL=schema-level | 1.11 CREATE ICEBERG TABLE syntax | 1.1 CS accrues without WH | 1.12 Anaconda packages | 1.5 Column-level Security=Enterprise | 1.9 Cortex Fine-tuning | 1.12 Streamlit in Notebooks
- Wrong answers: Q17 (Shares = ACCOUNT-level, not schema-level) | Q20 (Storage Integration = ACCOUNT-level, not schema-level) | Q25 (SQL API = REST-based; confused with ODBC)
- **NEW TOPICS MASTERED: 1.5 Snowflake Editions ⭐ (11/12=92%) · 1.9 AI/ML Features ⭐ (8/8=100%) · 1.12 Snowflake Notebooks ⭐ (8/8=100%)**
- 🏅 **LEVEL UP: Level 10 → Level 11 — Domain Specialist** 🎉 (coverage crossed 68% gate mid-drill)
- 🏅 **SNOPRO READY BADGE UNLOCKED** ⭐ — 313/447 = 70% coverage with 84% accuracy!
- Coverage: 288 → **313/447 (70.0%)** — 70% TARGET REACHED! ✅ | Mastered topics: 5 → **8/46**
- Domain Architecture: 67 → 92/115 (58% → **80%**)
- Per-domain accuracy: Arch 93/111 (84%) → **120/141 (85%)** | Total 413/493 → **440/523 (84%)**
- Topic updates: 1.1 60%→80% | 1.3 60%→70% | 1.4 50%→60% | 1.5 50%→92%⭐ | 1.6 50%→63% | 1.8 50%→70% | 1.9 63%→100%⭐ | 1.10 63%→88% | 1.11 44%→78% | 1.12 38%→100%⭐
- XP: 9338→**9973** | Questions: 680→**710** | Exam date: unchanged (June 8 — target reached, on schedule!)
- Persistent confusion: 1.7 object hierarchy — Shares AND Storage Integrations are ACCOUNT-level (both Q17+Q20 wrong on this pattern; already bookmarked from S9/S11)

### CertSafari — 2026-05-30 (50 questions, external)
- Score: 45/50 (90%) | ⚠️ Q29 = site error (identical user/correct answers shown) → effective 46/50 (92%)
- Source: CertSafari (no XP awarded)
- New sub-concepts: +11 net (no removals — all wrong answers hit uncovered sub-concepts)
- Added: 1.1 Cloud Services re-added | 1.2 Snowpark-optimized WH memory | 1.2 ALTER WAREHOUSE resize syntax | 3.1 RESULT_SCAN | 3.1 CTE WITH clause | 3.1 GROUP BY + HAVING | 3.2 USE_CACHED_RESULT = FALSE | 4.6 .NET/Go/Node.js connectors | 5.1 Resharing | 5.2 Free listing billing | 5.4 Clone copies TT data + masking policies
- Wrong answers: Q5 (External Function for REST API — picked Storage Integration) | Q9 (API INTEGRATION prereq for External Functions — picked Stream) | Q22 (SOS for point lookups — picked clustering key; recurring confusion) | Q32 (Git repo FETCH + CREATE OR REPLACE — picked auto-detect)
- Q44 confirmed correct: Option B = "TT retention > 1 day not available for transient" (transcription error earlier misread as > 0 days; > 1 day is accurate — transient max = 1 day TT; already covered sub-concept)
- Per-domain (quiz mapping): Arch 9/9 (100%) | Gov 10/10 (100%) | Perf 10/11 (91%, Q22 wrong) | Load 6/9 (67%, Q5/Q9/Q32 wrong) | Collab 11/11 (100%)
- **NEW TOPICS MASTERED: 3.1 Query Profile ⭐ (10/10 = 100%) | 5.1 Secure Data Sharing ⭐ (9/10 = 90%)**
- Coverage: 277 → **288/447 (64.4%)** | Mastered topics: 3 → **5/46**
- Domain updates: Arch 64→67/115 (58%) | Perf 36→40/66 (61%) | Load 43→44/79 (56%) | Collab 44→47/81 (58%) | Gov unchanged 87/106 (82%)
- Exam date recalculated: June 5 → **June 8** (rolling avg: S18=-3, CS-May29=+15, CS-May30=+11 → 7.7/session × 2/day = 15.3/day; target 313/447 → 25 remaining ÷ 15.3 + 7 buffer = 8.6 days)
- XP: unchanged (9338) | Questions: 630 → **680**
- Persistent weak spots: External Functions concept (new — 2 wrongs), SOS vs clustering key (3+ wrongs), Git integration (new miss)
- New bookmarks: External Functions / API INTEGRATION distinction | Git repository FETCH + CREATE OR REPLACE flow

### CertSafari Mock — 2026-05-29 (50 questions, external)
- Score: 49/50 (98%) — highest mock score to date
- Source: CertSafari (no XP awarded)
- New sub-concepts: ~15 added, 1 removed + 1 replaced = **+15 net**
- Removed: ~~5.3: Secondary replica database is read-only; available cross-region and cross-cloud; all editions~~ (Q19 wrong — confused with failover)
- Key additions: FLATTEN() | SPLIT()+FLATTEN() | Scalar UDF vs UDTF | RANK() window function | SOS "Search Optimization Access" node in Query Profile | Result cache conditions (data unchanged + exact match + access privileges) | LIST @stage | Parameter precedence (Session > User > Account) | Suspended warehouse = 0 credits | ALERT schema-level object | Secondary replica queryable without failover (clearer re-add) | Marketplace provider steps | Dynamic Table incremental refresh | Object owner privileges (GRANT/DROP/transfer) | Marketplace consumer can request datasets
- Wrong answers: Q19 (secondary replica — thought failover needed to query; actually directly queryable read-only, just needs USAGE + warehouse)
- Q6 confirmed correct: 20-second query on resumed warehouse → billed for 60 seconds (minimum billing period at startup); already a covered sub-concept (1.2)
- Per-domain (CertSafari): Arch 11/11 (100%) | Gov 10/10 (100%) | Load 9/9 (100%) | Perf 11/11 (100%) | Collab 8/9 (89%)
- Coverage: 262 → **277/447 (61.9%)** — crosses 60% ✅
- Domain updates: Arch 60→64/115 (56%) | Gov 85→87/106 (82%) | Perf 32→36/66 (55%) | Load 40→43/79 (54%) | Collab 42→44/81 (54%)
- XP: unchanged (8563 → still 9338) | Questions: 580→**630** | Exam date: no change (v2 coverage-based, recalculate next session)

### Session 18 — Historical Wrong Answer Review — 2026-05-28 (43 questions)
- Score: 33/43 (77%)
- XP delta: +775 XP
- Best streak this session: 12 (Q9–Q20) | All-time best streak: 22
- Sub-concepts: 6 removed, 3 re-added = **-3 net** (265 → 262/447)
- Removed: ~~2.3 IdP issues SAML assertion~~ (Q1 wrong — SAML/OAuth confusion 4th instance) | ~~2.5 ALTER TABLE ALTER COLUMN SET MASKING POLICY~~ (Q8) | ~~3.7 QAS SELECT-only~~ (Q35) | ~~3.5 ALTER TABLE ADD SEARCH OPTIMIZATION~~ (Q40) | ~~3.7 ALTER WAREHOUSE ENABLE_QUERY_ACCELERATION~~ (Q41) | ~~1.3 micro-partition metadata includes DISTINCT COUNT~~ (Q43)
- Re-added: 3.2 result cache in Cloud Services layer | 3.2 result cache account-wide | 2.3 SAML assertion = XML format (distinct from IdP sub-concept)
- Wrong answers: Q1 (SAML/OAuth — picked OAuth for SSO scenario) | Q3 (ALTER ACCOUNT SET NETWORK_POLICY — picked APPLY ON ACCOUNT again) | Q8 (DDM syntax — picked SET…ON COLUMN) | Q21 (ACCOUNT_USAGE.TABLES vs TABLE_STORAGE_METRICS) | Q32 (Parquet+ORC columnar — missed Parquet, picked ORC+Avro) | Q35 (QAS SELECT only — also picked INSERT…SELECT) | Q39 (Iceberg = Parquet — picked ORC) | Q40 (SOS ADD syntax — picked ENABLE) | Q41 (QAS per warehouse — picked query-level hint) | Q43 (micro-partition metadata — missed DISTINCT COUNT)
- ⚠️ Persistent failures: SAML/OAuth (4 wrongs), ALTER ACCOUNT SET NP (3 wrongs), SOS/QAS syntax (2 wrongs each this session)
- Per-domain accuracy this session: Gov 17/21 (81%) | Arch 9/11 (82%) | Perf 3/7 (43%) | Load 1/1 (100%) | Collab 3/3 (100%)
- Topics updated: 1.3 6→5/10 (50%) | 2.3 9→8/12 (67%) | 2.5 11→10/15 (67%) | 3.2 +2 re-added | 3.5 5→4/9 (44%) | 3.7 5→3/9 (33%)
- Exam date: no change (77% = 70-79% band) → **June 5**
- XP: 8563→**9338** | Sub-concepts: 265→**262**/447 (58.6%) | Questions: 537→**580**
- Note: APPROX_COUNT_DISTINCT metadata usage disputed — bookmarked for doc verification

### Session 17 — Governance 30 — 2026-05-28 (30 questions)
- Score: 26/30 (87%)
- XP delta: +678 XP
- Best streak this session: 14 (Q7–Q20) | All-time best streak: 22
- New sub-concepts: 15 added, 1 removed (SAML SSO confused with OAuth — 3rd instance of this confusion) = **+14 net**
- Added: 2.5 DDM syntax | 2.7 TLS 1.2+ | 2.5 EXEMPT MASKING POLICY | 2.5 one masking policy/column | 2.2 USERADMIN→SECURITYADMIN hierarchy | 2.3 Authentication Policy | 2.5 DDM masks WHERE | 2.6 tag propagation | 2.5 one RAP/table | 2.10 APPLY privilege for projection policy | 2.6 database role scope | 2.1 ACCOUNTADMIN 2-3 users | 2.10 privacy policies schema-level | 2.3 OAuth token claims | 2.3 IdP issues SAML assertion
- Wrong answers: Q3 (SAML SSO — picked OAuth) | Q6 (ALTER ACCOUNT SET NETWORK_POLICY — picked APPLY ON ACCOUNT) | Q21 (SAML assertion — picked JWT) | Q22 (ALTER ACCOUNT SET NETWORK_POLICY re-test — still wrong)
- 🏅 **LEVEL UP: Level 9 → Level 10 — Collaboration Pro** 🎉 (coverage 57.97% → 59.3%; XP 7885 → 8563)
- ⭐ **2.2 Role Hierarchy MASTERED** — 9/9 = 100% (third topic to reach mastery!)
- Per-domain accuracy: Gov 26/30 (87%)
- Topics updated: 2.1 9→10/12 (83%) | 2.2 8→9/9 (100%) ⭐ | 2.3 7→9/12 (75%) | 2.5 6→11/15 (73%) | 2.6 6→8/10 (80%) | 2.7 7→8/11 (73%) | 2.10 6→8/10 (80%)
- Gov overall: 73/92 → **87/106 (82%)**
- Persistent weak spots: SAML SSO vs OAuth (3 wrongs total), ALTER ACCOUNT SET NETWORK_POLICY syntax (2 wrongs this session) — must drill these next session
- XP: 7885→**8563** | Sub-concepts: 251→**265**/447 (59.3%) | Questions: 507→**537**
- Exam date: June 6 → **June 5** (score 87%, 80-89% → 1 day closer)

### Session 16 — Governance Drill Round 2 — 2026-05-27 (10 questions)
- Score: 8/10 (80%)
- XP delta: +180 XP (8 correct × 20 XP + streak bonus Q7–Q10 ×5 = +20; streak built Q5→Q10, hit 3 at Q7)
- New sub-concepts: 8 net [NEW: Q1 re-added, Q2 re-added, Q5, Q6, Q7, Q8, Q9, Q10]
- Added: 2.10 Projection NULLIFY re-added | 2.1 SECURITYADMIN re-added | 2.3 RSA_PUBLIC_KEY syntax | 2.4 BLOCKED_IP_LIST | 2.10 aggregation policy level | 2.6 APPLY privilege | 2.1 Managed Access Schema | 2.10 Projection FAIL mode
- Wrong answers: Q3 (EXEMPT MASKING POLICY, not OVERRIDE — account-level privilege to bypass all DDM policies) | Q4 (TLS 1.2+ for in transit, not RSA-4096; RSA is key exchange inside TLS)
- Per-domain: Gov 8/10 (80%)
- Topics updated: 2.1 7→9/12 (75%) | 2.3 6→7/9 (78%) | 2.4 5→6/8 (75%) | 2.6 5→6/8 (75%) | 2.10 3→6/8 (75%)
- 🏅 **MARATHON BADGE UNLOCKED** — 507 questions answered (500+ threshold)
- XP: 7705→**7885** | Sub-concepts: 243→**251**/433 (57.97%) | Questions: 497→**507**
- Level 10 gate: XP met (7885 > 5500); coverage 57.97% — **1 sub-concept away from 58%** 👀

### Session 16 — Governance Drill Round 1 — 2026-05-27 (10 questions)
- Score: 7/10 (70%)
- XP delta: +164 XP (7 correct × 20 XP + streak bonus Q7–Q8 = +10; streak resets at Q3/Q4 wrong, picks back up Q5)
- New sub-concepts: 6 net | 1 reinforcement [NEW: Q2, Q5, Q6, Q7, Q8, Q10 | REINFORCED: Q1]
- Added: 2.10 MIN_GROUP_SIZE suppression | 2.5 RAP ALTER TABLE ADD syntax | 2.5 RAP schema-level | 2.1 ORGADMIN | 2.4 ALLOWED_IP_LIST | 2.3 Password Policy
- Reinforced: 2.10 Aggregation policy purpose (Q1 — already covered, no new coverage)
- Wrong answers: Q3 (projection policy — NULLIFY mode returns NULL, FAIL mode aborts query; both are valid enforcement modes) | Q4 (DDM syntax = ALTER TABLE t ALTER COLUMN col SET MASKING POLICY p — SET not ADD) | Q9 (Tri-Secret = AWS KMS + Azure Key Vault + GCP Cloud KMS — all 3 providers; answered B only)
- Per-domain: Gov 7/10 (70%)
- Topics updated: 2.1 6→7/12 (58%) | 2.3 5→6/9 (67%) | 2.4 4→5/8 (63%) | 2.5 4→6/10 (60%) | 2.10 2→3/8 (38%)
- Note: Projection policy TWO enforcement modes — NULLIFY (SELECT returns NULL, WHERE uses real data) and FAIL (query errors entirely); DDM masks in WHERE clause too, making DDM stronger against inference attacks
- XP: 7541→**7705** | Sub-concepts: 237→**243** / 433 (56.1%) | Questions: 487→**497**

### Mock Exam Round 2 — 2026-05-27 (19 questions, external — part 2 of 50)
- Score: 18/19 (95%)
- Source: External mock exam (no XP awarded)
- New sub-concepts: 8 net (9 added, 1 removed — SECURITYADMIN MANAGE GRANTS confusion recurs)
- Added: 5.1 Direct Share | 3.7 ALTER WH ENABLE_QUERY_ACCELERATION | 2.6 tags on securable objects | 3.3 workload isolation | 5.7 overlap analysis technique | 3.5 SOS dual billing | 2.8 tags for cost allocation | 2.8 RM properties (quota/frequency/actions) | 2.2 USE ROLE session
- Removed: 2.1 SECURITYADMIN MANAGE GRANTS (wrong for 3rd time — Q2; pattern: confusion with SYSADMIN)
- Wrong answers: Q2 (SECURITYADMIN has MANAGE GRANTS, not SYSADMIN — SYSADMIN manages data objects)
- Per-domain: Arch 1/1 (100%) | Gov 6/7 (86%) | Perf 4/4 (100%) | Load 2/2 (100%) | Collab 5/5 (100%)
- New topic mastered: 2.8 Cost Management & Monitors (10/10 = 100%) ⭐
- Combined mock exam (50 Q): 43/50 (86%) | 18 net new sub-concepts (219→237)

### Mock Exam Round 1 — 2026-05-27 (31 questions, external — part 1 of ~50)
- Score: 25/31 (81%)
- Source: External mock exam (no XP awarded)
- New sub-concepts: 10 (219 → 229) — 1.2 CREATE WAREHOUSE DDL | 1.6 ODBC driver | 1.7 Sequences NEXTVAL | 2.6 Context Functions | 2.7 internal stage AES-128/256 | 2.8 QUERY_HISTORY for DDL audit | 4.2 ON_ERROR=ABORT_STATEMENT default | 4.2 COPY INTO @stage unloading | 5.1 CREATE DATABASE FROM SHARE | 5.1 ALTER SHARE ADD ACCOUNTS
- Wrong answers: Q1 (Always-on Encryption ≠ End-to-End Encryption; Always-on = Snowflake's term for non-configurable AES-256 at rest) | Q18 (.NET app → ODBC driver, not Python Connector — Python Connector is Python-only) | Q21 (ROW_SEPARATOR not valid CSV option; correct param is RECORD_DELIMITER) | Q24 (Marketplace listing IS a wrapper over Secure Data Sharing, not a separate feature) | Q26 (CORTEX.EXTRACT_ANSWER for Q&A from a document; CORTEX.COMPLETE for open-ended LLM generation) | Q30 (per-query credit cost → QUERY_HISTORY.CREDITS_USED; WAREHOUSE_METERING_HISTORY is per-warehouse totals only)
- Per-domain: Arch 6/8 (75%) | Gov 5/7 (71%) | Perf 3/3 (100%) | Load 7/8 (88%) | Collab 4/5 (80%)
- 19 more questions incoming (full batch recap pending)

### CertSafari Mixed Drill — 2026-05-26 (10 questions)
- Score: 8/10 (80%)
- Source: CertSafari mixed practice (external, no XP awarded)
- New sub-concepts: 3 (216 → 219) — Q1, Q2, Q4, Q7, Q8 already covered; Q3, Q10 wrong (not added)
- Wrong answers: Q3 (Snowflake Extension for VS Code ≠ SnowSQL; SnowSQL is CLI-only, Extension integrates into IDE) | Q10 (Cortex Search = unified search across structured + unstructured; Cortex Analyst = conversational structured-only)
- Per-domain: Arch 6/8 (75%) | Perf 2/2 (100%)
- Architecture crosses 50% coverage (58/115)! 📊
- Skip next session (add to S16 list): Snowflake Extension for VS Code (IDE plugin, not CLI), Cortex Search vs Cortex Analyst distinction

### CertSafari Governance Drill 2 — 2026-05-26 (10 questions)
- Score: 9/10 (90%)
- Source: CertSafari Governance-focused practice (external, no XP awarded)
- New sub-concepts: 5 (211 → 216) — Q5, Q6, Q7, Q9 already covered; Q4 wrong (not added)
- Wrong answers: Q4 (user session is NOT a securable object — virtual warehouses ARE; can't GRANT privileges ON a session)
- Per-domain: Gov 9/10 (90%)
- ⭐ **2.9 Data Lineage MASTERED** — 8/8 = 100% (first topic to reach mastery!)
- Governance accuracy: 67% → **70%** (43/64 → 52/74)
- Skip next session (add to S16 list): user session = not a securable object; securable objects are things you can GRANT ON (warehouses, databases, tables, schemas, roles, etc.)

### CertSafari Governance Drill — 2026-05-26 (10 questions)
- Score: 7/10 (70%)
- Source: CertSafari Governance-focused practice (external, no XP awarded)
- New sub-concepts: 5 (206 → 211) — Q5 and Q7 already covered; Q3, Q6, Q9 wrong (not added)
- Wrong answers: Q3 (database role scoped to single DB, not account role = users-only) | Q6 (ALERT = scheduled condition + action; not Resource Monitor which is credit-spend only) | Q9 (TABLES IS in ACCOUNT_USAGE; confused with DATABASE_STORAGE_USAGE_HISTORY)
- Per-domain: Gov 7/10 (70%)
- Level up: 8 → **9 — Pipeline Builder** 🆙 (coverage 47.6% → 48.7% crossed 48% gate; XP gate already met)
- Skip next session (add to S16 list): database role scope (confined to single DB), ALERT vs Resource Monitor distinction, TABLES view in ACCOUNT_USAGE

### CertSafari Architecture Drill — 2026-05-26 (9 questions)
- Score: 8/9 (89%)
- Source: CertSafari Architecture domain (external, no XP awarded)
- New sub-concepts: 2 (204 → 206)
- Wrong answers: Q2 (smallest warehouse = X-SMALL, not SMALL)
- Per-domain: Arch 8/9
- Notes: Confused X-Small as smallest size. ML components (Feature Store, Modeling API, Model Registry) now covered. Micro-partition pruning solid — correctly explained why clustering key on col A doesn't help prune col B.

### CertSafari External — 2026-05-26 (50 questions)
- Score: 43/50 (86%)
- Source: CertSafari practice exam (external, no XP awarded)
- New sub-concepts: 10 net (11 added, 1 removed — transient TT confused with external)
- Wrong answers: Q6 (Python Connector for Python scripts, not Snowsight) | Q7 (objects_modified column in ACCESS_HISTORY for write lineage) | Q14 (GCS trust = STORAGE_GCP_SERVICE_ACCOUNT + STORAGE_ALLOWED_LOCATIONS) | Q18 (TT NOT available on Temporary + External — Transient HAS TT!) | Q19 (Snowsight worksheets can be shared with other users) | Q33 (SYSTEM$CLUSTERING_INFORMATION + SYSTEM$CLUSTERING_DEPTH) | Q42 (ML Model = schema-level object)
- Per-domain: Arch 8/11 (73%) | Gov 7/8 (88%) | Perf 10/11 (91%) | Load 8/9 (89%) | Collab 11/11 (100%)
- Key confusion: Transient vs External for Time Travel availability — Transient HAS 1-day TT, External has NONE
- Notes: Architecture weakest (3 wrong: interfaces, table types, object hierarchy). Governance much stronger externally (88%) than in our sessions (67% cumulative). Load streak broken by GCS integration detail.

### Session 15 — 2026-05-26 (Weak Spots — 22 questions)
- Score: 18/22 (82%) — Q7 voided (ambiguous + skip-list item, full credit given)
- XP delta: +458 XP
- Best streak this session: 11 (Q6–Q16) | All-time best streak: 22
- New sub-concepts: 11 net (12 added, 1 removed — projection policy NULL)
- Wrong answers: Q5 (RAP = schema-level, not account-level) | Q17 (ALTER TABLE ADD ROW ACCESS POLICY, not SET) | Q18 (projection policy → WHERE works normally, SELECT returns NULL not excluded) | Q21 (key-pair auth public key via ALTER USER ... SET RSA_PUBLIC_KEY, not embedded in connection string)
- Level: no change (8 — Performance Practitioner); need 14 more sub-concepts for Level 9 (48% coverage)
- Exam date: June 2 → June 5 (recalculated from 2026-05-26; rolling avg S13=39, S14=10, S15=11 → 20/session × 2/day = 40/day; 109 remaining ÷ 40 = 2.7 + 7 buffer = ~10 days)
- Per-domain accuracy (S11+ ledger): Arch 35/43 81% | Gov 29/46 63% | Perf 20/25 80% | Load 19/19 100% | Collab 22/28 79%
- Skip next session (S16): RAP = schema-level object, ALTER TABLE ADD ROW ACCESS POLICY syntax, projection policy behavior in WHERE (returns NULL in SELECT), ALTER USER SET RSA_PUBLIC_KEY for key-pair auth

### Session 14 — 2026-05-23 (Weak Spots — 50 questions)
- Score: 38/50 (76%)
- XP delta: +1154 XP
- Best streak this session: 7 | All-time best streak: 22
- New sub-concepts: 10 net (13 added, 3 removed)
- Wrong answers: Q1 (agg policy suppresses groups, not error) | Q2 (sharing = direct read, no copy) | Q3 (Cloud Services = query opt/metadata/access control) | Q11 (agg policy attachment = SET not ADD) | Q12 (SOS = equality only, not range) | Q20 (MIN_GROUP_SIZE parameter name) | Q23 (result cache = Cloud Services layer, not Storage) | Q28 (APPLY privilege for masking policy) | Q36 (result cache account-wide, not WH-specific) | Q41 (VWH cannot be cloned) | Q45 (agg policy at table/view level, not column) | Q50 (columnar = Parquet + ORC only, not Avro)
- Level up: 7 → 8 (Performance Practitioner) at Q22 — coverage crossed 40%
- Level 9 gate: XP met (7091 > 4000), need 26 more sub-concepts for 48% coverage
- Exam date: June 1 → June 2 (rolling avg S12=7, S13=39, S14=10 → avg 19/session; 121 remaining at 38/day = 3.2 + 7 buffer)
- Per-domain accuracy (S11+ ledger): Arch 31/39 79% | Gov 24/37 65% | Perf 15/20 75% | Load 18/18 100% | Collab 20/26 77%
- Skip next session (S15): agg policy group suppression, secure sharing = direct read, Cloud Services = query opt/metadata/access control, agg policy SET syntax, SOS equality-only predicates, MIN_GROUP_SIZE parameter name, result cache = Cloud Services layer, APPLY privilege for masking, result cache account-wide not WH-specific, VWH cannot clone, agg policy at table/view level, columnar = Parquet+ORC only (not Avro)

### Session 13 — 2026-05-22 (Weak Spots — 50 questions)
- Score: 41/50 (82%)
- XP delta: +1273 XP
- Best streak this session: 18 (Q21–Q38) | All-time best streak: 22
- New sub-concepts: 39 (133 → 172)
- Wrong answers: Q6 (secure views only in shares) | Q11 (RAP = schema-level object) | Q12 (consumer grants IMPORTED PRIVILEGES) | Q16 (QAS = SELECT queries only) | Q20 (HIPAA/PCI = Business Critical, not VPS) | Q39 (Cloud Services = transaction management) | Q46 (SCIM = IdP user/group provisioning, not session management) | Q48 (masking USING clause = additional column context, not encryption algorithm) | Q50 (Iceberg data files = Parquet format)
- Level up: 6 → 7 (Governance Learner) at Q10 — coverage crossed 32%
- Level 8 gate: XP met (5937 > 3000), need 2 more sub-concepts for 40% coverage
- Exam date: June 3 → June 1 (rolling avg S11=23, S12=7, S13=39 → avg 23/session; 131 remaining at 46/day)
- Per-domain accuracy (S11+ ledger): Arch 21/27 78% | Gov 17/24 71% | Perf 11/14 79% | Load 12/12 100% | Collab 13/17 76%
- Skip next session (S14): secure views in shares, RAP schema-level, IMPORTED PRIVILEGES, QAS SELECT-only, HIPAA=Business Critical, Cloud Services=transaction management, SCIM=IdP provisioning, masking USING clause, Iceberg=Parquet

### Session 12 — 2026-05-22 (Weak Spots — stopped at 15 questions)
- Score: 10/15 (67%) — planned 50, interrupted; Q13 voided (ambiguous question, full credit given)
- XP delta: +140 XP
- Best streak this session: 3 | All-time best streak: 22
- New sub-concepts: 7 (126 → 133)
- Wrong answers: Q3 (SOS = ALTER TABLE...ADD SEARCH OPTIMIZATION, not SET) | Q7 (QAS = ALTER WAREHOUSE...SET ENABLE_QUERY_ACCELERATION per warehouse, not account) | Q9 (Application Package = provider-side container for app definition + releases) | Q11 (EXEMPT MASKING POLICY bypasses DDM, not OVERRIDE) | Q12 (Aggregation policy suppresses results below min entity count — not mandatory GROUP BY)
- Level: no change (6 — Architecture Explorer); 6 sub-concepts to Level 7
- Exam date: June 1 → June 3 (+2 days; rolling avg S10=18, S11=23, S12=7 → 16/session; 170 remaining at 32/day = 12.3 days + buffer)
- Per-domain accuracy (S11+ ledger): Arch 12/15 80% | Gov 8/12 67% | Perf 3/5 60% | Load 5/5 100% | Collab 5/7 71%

### Session 11 — 2026-05-20 (Weak Spots — 30 questions)
- Score: 24/30 (80%)
- XP delta: +687 XP
- Best streak this session: 6 | All-time best streak: 22
- New sub-concepts: 23 (103 → 126)
- Wrong answers: Q10 (external tables shareable in shares) | Q17 (Iceberg: Snowflake manages catalog for Snowflake-managed Iceberg tables) | Q20 (micro-partition metadata includes distinct count, not just min/max) | Q22 (projection policy → column returns NULL, not excluded entirely) | Q23 (all connectors support SQL execution; only SnowSQL supports PUT/GET) | Q30 (Network Rule is the schema-level object for defining IP ranges)
- Level up: 5 → 6 (Architecture Explorer) at Q6 — coverage crossed 25%
- Exam date: June 2 → June 1 (rolling avg 19.7/session × 2/day = 39.3/day, 177 remaining)

### Session 10 — 2026-05-19 (Weak Spots — 20 questions)
- Score: 18/20 (90%)
- XP delta: +429 XP (18×20 + 2×2 wrong + streak bonuses Q3-Q5 ×5=15, Q11-Q20 ×5=50 → +65)
- Best streak this session: 12 (Q9–Q20)
- New sub-concepts: 3.4 overlap_depth, 3.5 SOS billing, 3.6 MV edition, 3.7 QAS query types, 3.3 MAX_CONCURRENCY_LEVEL, 2.7 AES-256, 2.10 projection policy, 2.6 RAP CURRENT_ROLE, 5.6 Snowflake Support only/transient no fail-safe, 5.7 Native App Framework, 5.8 Marketplace distribution, 1.9 ML.FORECAST, 1.12 SQL+Python+Markdown, 4.3 INFER_SCHEMA/MATCH_BY_COLUMN_NAME, 4.7 GET command, 5.2 Data Exchange (18 new)
- Wrong answers: Q6 MV transparent optimizer (thought explicit ref required) | Q8 rekeying edition (picked BC, correct = Enterprise)
- Doc correction: Periodic rekeying = Enterprise+, NOT Business Critical
- Exam date: June 4 → June 2 (rolling avg 14.7/session × 2/day = 29.3/day, 200 remaining)

### Sessions 1–9 (archived — detail rolled up into Current State)
| Session | Date | Mode | Score | XP | Notes |
|---|---|---|---|---|---|
| S1 | 2026-05-16 | Rapid 21 | 19/21 (90%) | +530 | Legacy binary mastery system |
| S2 | 2026-05-16 | Rapid 10 | 9/10 (90%) | +172 | Coverage system begins; XP recalculated from +337 (removed exponential bonuses) |
| S3 | 2026-05-16 | Rapid 10 | 7/10 (70%) | +156 | XP recalculated from +181 |
| S4 | 2026-05-16 | Rapid 10 | 8/10 (80%) | +184 | XP recalculated from +217 |
| S5 | 2026-05-17 | Rapid 10 | 9/10 (90%) | +205 | |
| S6 | 2026-05-17 | Mock (Q20/100) | 17/20 (85%) | +391 | Level up L6 |
| S7 | 2026-05-17 | Weak Spots 10 | 8/10 (80%) | +189 | |
| S8 | 2026-05-18 | Rapid 50 | 47/50 (94%) | +1121 | Level up; Century Club badge; all-time streak 22 |
| S9 | 2026-05-18 | Weak Spots 20 | 18/20 (90%) | +452 | Level up L5; Q15 voided (bad question wording) |

---

## Session — 2026-06-01 (S-Jun01a) — Weak Spots 10
- Overall: 9/10 correct (90%) *(Q5 credit adjusted — mobile truncation)*
- XP earned: +185 XP
- Total XP: 10158 | Level 11: Domain Specialist
- Overall coverage: ~71.4% (330/462)
- Exam readiness: 84%
- Best streak this session: 5
- All-time best streak: 22
- Total questions answered: 770
- Badges earned: none new
- Domain focus: Performance, Data Loading, Collaboration (weak spots)
- Wrong: Q5 partial (DATA_RETENTION option truncated on mobile — credited)
- Notes: Mobile display issue — long option labels get cut off. Keep labels short.

---

## Session — 2026-06-01 (S-Jun01b) — 50-Question Weighted Quiz
- Overall: 39/45 correct (87%) *(5 questions dismissed/interrupted)*
- XP earned: +912 XP
- Total XP: 11070 | Level 11: Domain Specialist (74.2% coverage — need 75% for L12!)
- Overall coverage: 74.2% (343/462)
- Exam readiness: 86%
- Best streak this session: 9
- All-time best streak: 22
- Total questions answered: 815
- Badges earned: none new (14 topics now mastered — up from 7!)
- Domain mastery:
  - Arch: 88% (103/117) — covered: 1.1⭐ 1.2⭐ 1.3⭐ 1.5⭐ 1.10⭐ 1.12⭐ | uncovered: 1.7 1.9
  - Gov: 87% (94/108) — covered: 2.1⭐ 2.2⭐ 2.6⭐ 2.8⭐ 2.9⭐ 2.10⭐ | uncovered: 2.4
  - Perf: 67% (46/69) — covered: 3.1⭐ | uncovered: 3.7
  - Load: 60% (50/84) — uncovered: 4.3
  - Collab: 60% (50/84) — covered: 5.1⭐ | uncovered: 5.4
- Final Boss unlocked: No (Perf 67%, Load 60%, Collab 60% — need all 80%+)
- Wrong answers: 1.7 storage integrations, 1.9 Snowpark languages (no R), 2.4 network policy syntax, 3.7 SYSTEM$ESTIMATE_QUERY_ACCELERATION, 4.3 unload formats (CSV/JSON/Parquet only), 5.4 clone contents (stages included, privileges not)
