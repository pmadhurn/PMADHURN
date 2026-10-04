# Madhur N Patel

**DevOps / infrastructure, embedded systems, backend.** Ahmedabad, India.
B.Tech Computer Science & Engineering, Indus University, 2022–2026.

I build things and then I keep them running. Everything linked below is live on one ARM64 Oracle Cloud server I
administer myself — **2 cores, 12 GB RAM, 200 GB disk, 40+ Docker containers, ~25 public services**, all reachable
through a Cloudflare Tunnel with **zero inbound ports open**. Nginx routing, systemd units, fail2ban, log rotation,
nightly backups, and Telegram alerts when something degrades. None of it is a tutorial copy — it broke, I fixed it,
that is how I learned.

**Open to work — first full-time role, available immediately.**
DevOps / Infrastructure / Platform / SRE first; embedded, robotics and backend close behind.
[madhur.dev](https://madhur.dev) · [LinkedIn](https://linkedin.com/in/madhur-n) · pmadhurn@gmail.com

---

## What's running right now

| | |
|---|---|
| **[NavDashboard](https://nav.madhur.dev)** | Asset & operations tracking — devices, inventory, personnel, QR labels, gate-pass workflows. Async FastAPI with a per-capability permission engine, local-LLM assistant, React 18 + TS, PostgreSQL + PostGIS + pgvector, Redis, MinIO. |
| **[PulseBoard](https://health.madhur.dev)** | My own monitoring: CPU, memory, swap, storage, network, disk I/O, processes. Zero-idle by design — it costs nothing when nobody is looking, which matters on a 2-core box that is also serving everything else. |
| **[Learn](https://learn.madhur.dev)** | Self-hosted AI tutor — streamed lessons with citations, adaptive quizzes with grading, multi-model routing with stall failover. |
| **Read** (`read.madhur.dev`, passcode-gated) | Family speed-reading library — shared shelf, RSVP reader, progress, streaks and leagues. Runs on the same box; link withheld because it holds family data. |
| **[FileDrop](https://link.madhur.dev)** | Anonymous chunked uploads, one short link, hard-deleted after 24 hours. |

## Projects

- **[SpeakInsights](https://github.com/pmadhurn/SpeakinsightsV6)** — on-premises meeting platform with no
  third-party API calls: LiveKit WebRTC for 20 participants, WhisperX transcription with speaker attribution,
  summaries from a local Ollama model, RAG chat over past meetings.
- **[ESP32 drone flight controller](https://github.com/pmadhurn/Drone)** — quadcopter firmware in C (ESP-IDF):
  MPU6050 attitude estimation with a complementary filter, ultrasonic altitude hold, angle-mode pitch/roll and
  rate-mode yaw PID with anti-windup, battery monitoring, failsafes for link loss / low battery / IMU failure /
  attitude limits, 20 Hz telemetry over a versioned UDP protocol. Flown from an
  [Android controller](https://github.com/pmadhurn/DroneController) I also wrote.
- **GPS-guided dual-device tracker** — two Raspberry Pi gimbals point at each other by GPS bearing, then hand off
  to OpenCV LED tracking for the alignment a GPS fix is too coarse for. 9-axis sensor fusion (GPS, IMU,
  magnetometer) under PID control.

## Stack

```
Infra        Linux (Ubuntu), Docker & Compose, Nginx, Cloudflare Tunnel, systemd,
             Oracle Cloud, AWS, GCP, GitHub Actions, Bash
Backend      Python, FastAPI, Node/Express, SQLAlchemy (async), WebSockets
Data & AI    PostgreSQL (PostGIS, pgvector), Redis, MongoDB, MySQL, MinIO,
             Ollama, WhisperX, RAG pipelines
Frontend     React 18, TypeScript, Vite, TailwindCSS, Ant Design, Zustand
Embedded     ESP32 (ESP-IDF, PlatformIO), Raspberry Pi 5/4/3, Pico, Arduino,
             C/C++, I2C, UART, PWM, OpenCV
```

AWS Academy: Cloud Foundations (Jul 2025) · Machine Learning Foundations (Aug 2025)
