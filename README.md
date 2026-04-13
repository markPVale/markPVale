# Mark Vale
Edge Systems Engineer · Firmware & Cloud Infrastructure

I come from high-scale e-commerce: distributed systems,
resilience patterns, observability at scale. I'm applying
that foundation to a harder problem: software that interacts
directly with the physical world, where failures are the norm
and correctness is non-negotiable.

---

## Current work

### Industrial Sensor Pipeline
`ESP32` · `C++` · `FreeRTOS` · `MQTT` · `InfluxDB` · `Grafana`

Retrofitting legacy industrial assets with deterministic edge
firmware. The hard problem: maintaining data integrity and
system correctness under unreliable connectivity, memory
pressure, and real-world failure conditions.

Core engineering challenges:
- PSRAM-backed ring buffer with drop-oldest eviction under pressure
- Edge-side backpressure with bounded queues and buffered replay on reconnect
- State machine recovery: NORMAL → BUFFERING → SYNCING,
  with boot_id and sequence tracking across disconnects

In progress: end-to-end backpressure propagation from cloud ingest to edge.

---

## Engineering approach

I design for the unhappy path. Edge cases, race conditions,
and failure modes under real-world pressure are where systems
either hold or collapse. Patterns from distributed systems:
backpressure, idempotency, fault isolation apply directly
to embedded firmware. The constraints are tighter. The
consequences are more immediate.

---

## Background

Five years building high-scale e-commerce infrastructure:
SSR architecture, transactional integrity, sub-second
performance at scale. The resilience patterns that protect
a distributed web system are the same ones that protect an
edge device under memory pressure.

---

[mark@markvale.dev](mailto:mark@markvale.dev) · [LinkedIn](https://linkedin.com/in/markvalestudio)
