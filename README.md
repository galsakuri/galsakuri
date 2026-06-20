# Hi, I'm Gal

**SOC Tier 2 Analyst · CS Student @ Holon Institute of Technology**

---

## About

Security analyst by day, but most of what I build sits closer to
infrastructure — containerized services, CI/CD pipelines, secret
management, and automation. Mostly Python, usually with a security angle.

---

## Projects

### CTI - Cyber Threat Intelligence Pipeline
*(built to support SOC work)*

Production pipeline, deployed and running 24/7. CI/CD on GitHub Actions
with a self-hosted runner (build, deploy, health-check on every push to
master) and CodeQL SAST in the pipeline. Hardened, non-root Docker image
under Compose, secrets in GCP Secret Manager with keyless service-account
auth. Failure-durable Python pipeline with a retry queue and a host-side
watchdog for container health, resource, and auth monitoring.
`Python · Docker · GitHub Actions · CodeQL · GCP Secret Manager · Vertex AI`

### [HomeSOC](https://github.com/galsakuri/HomeSOC)
Agent-based security monitoring platform for macOS. A local agent collects
security events and streams them to a FastAPI backend running a YAML
detection rule engine; a React/TypeScript dashboard shows a live feed and
per-agent config. Multi-service, Docker Compose, one-command bring-up.
`Python · FastAPI · React · TypeScript · SQLite · Docker Compose · GitHub Actions`

---

## Other Projects

| Project | Tech |
|:---|:---|
| [flight-price-checker](https://github.com/galsakuri/flight-price-checker) | Python · Amadeus API · SMTP |
| [stock-market-viewer](https://github.com/galsakuri/stock-market-viewer) | Python · Tkinter · Requests |
| [spotify-release-radar](https://github.com/galsakuri/spotify-release-radar) | Python · Spotipy · OAuth |
| [multi-user-chat-server](https://github.com/galsakuri/multi-user-chat-server) | Python · sockets · threading |

---

## Tech Stack

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/C-00599C?logo=c&logoColor=white"/>
  <img src="https://img.shields.io/badge/SQL-003B57?logo=sqlite&logoColor=white"/>
  <img src="https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white"/>
  <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?logo=githubactions&logoColor=white"/>
  <img src="https://img.shields.io/badge/FastAPI-009688?logo=fastapi&logoColor=white"/>
  <img src="https://img.shields.io/badge/GCP-4285F4?logo=googlecloud&logoColor=white"/>
  <img src="https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black"/>
  <img src="https://img.shields.io/badge/Git-F05032?logo=git&logoColor=white"/>
  <img src="https://img.shields.io/badge/Splunk-000000?logo=splunk&logoColor=white"/>
</p>

---

[LinkedIn](https://www.linkedin.com/in/gal-sakuri/)
