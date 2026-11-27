# NetShield-X

Intelligent Network Threat Detection & SOC Platform (Mini-SIEM).

منصة تجمع سجلات الشبكة من Suricata وZeek، تعالجها في Backend، تخزنها في PostgreSQL، وتعرضها للمحلل عبر Dashboard.

## Data Flow
GNS3 -> Linux Sensor -> Suricata / Zeek -> Log Collector -> FastAPI -> PostgreSQL -> React Dashboard

## Structure
| Folder | Purpose |
|---|---|
| network-lab/ | GNS3 topology and network configs |
| security/ | Suricata, Zeek, and the log collector |
| backend/ | FastAPI app, API, detection, models |
| database/ | PostgreSQL schema and migrations |
| frontend/ | React dashboard |
| shared/event-schema/ | Unified event JSON schema |

## Team Workflow
1. Never push directly to `main`.
2. Each member works on their own branch: `feature/<module-name>`.
3. Open a Pull Request; at least one teammate reviews before merge.
4. Weekly integration (not at the end of the project).
5. Every module has its own README explaining how to run it.
6. Never commit passwords, keys, or `.env` files.

## Team
| Member | Module |
|---|---|
| TBD | Network Infrastructure |
| TBD | Security Monitoring |
| TBD | Backend Core |
| TBD | Data & Detection |
| TBD | Frontend & Integration |
