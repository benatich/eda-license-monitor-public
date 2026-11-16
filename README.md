# EDA License Monitor

**Offline • Read-only • FlexNet License Monitoring**

A lightweight, Python-based monitoring solution for EDA license environments, including Cadence, Synopsys and Siemens EDA/MGC.

Designed for engineering and infrastructure teams that need visibility into license consumption without introducing complex dependencies.

## Dashboard Preview

*Dashboard preview using synthetic data — no production information.*

<img width="1600" height="910" alt="image" src="https://github.com/user-attachments/assets/64ebf0c6-476d-4f26-9a22-97a73330f09c" />


## Key Features

- **License Monitoring:** Observe issued, used and available licenses.
- **User Visibility:** Explore observed license sessions.
- **Historical Analytics:** Review utilization trends over 24 hours, 7 days and 30 days.
- **System Health:** Monitor source collection status and snapshot freshness.
- **CSV Export:** Export monitoring data for further analysis.
- **Offline Operation:** No external cloud services or Python dependencies.
- **Read-only Architecture:** No license checkout, release or server modification operations.

## Architecture

**M01 — Collector**

Periodic FlexNet status collection and local JSON snapshots.

**M02 — Dashboard**

Local web dashboard with Overview, Licenses, Users, Analytics and System Health.

**M03 — Alerting Engine**

Planned: configurable thresholds, stale-data detection and notifications.

## Compatibility

- Python 3.9+
- Linux
- Validated on RHEL 9.5
- FlexNet-based EDA license environments

## Security

The dashboard is designed for localhost access only. Authentication and HTTPS are not built in.

External access requires additional security controls.

## Project Status

**v0.2.0 — M02 Dashboard validated**

This repository is a public presentation of the project. It does not contain production configuration, real license snapshots or internal infrastructure information.

## Roadmap

- [x] M01 — License Collector
- [x] M02 — Web Dashboard
- [x] M02 — Security Hardening
- [ ] M03 — Alerting and Notifications
- [ ] Public demonstration with synthetic data

---

**EDA License Monitor — Built for visibility, simplicity and offline environments.**
