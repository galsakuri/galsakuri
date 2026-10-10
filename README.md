# Gal Sakuri

**Cyber Security Analyst** · detection engineering, incident response, security automation

B.Sc. Computer Science, Holon Institute of Technology (2026)

## About

I work as a Tier 2 SOC analyst. I write and tune Splunk and CrowdStrike detections mapped to MITRE ATT&CK,
investigate escalated incidents, and build tools the team uses every day. Most of that is Python, shipped in containers
through CI/CD.

## Work projects

The code for these is private. They run in production at work.

### CTI pipeline
A 24/7 pipeline that flags actively exploited CVEs from open-source feeds, so the SOC learns about live exploitation
the same day. Gemini on Vertex AI enriches each item and extracts IOCs. ChromaDB embeddings match reports of the same
threat across sources. Outbound fetches are checked against SSRF: a DNS lookup before every request and redirect, with private,
loopback, and cloud-metadata ranges blocked. It deploys through GitHub Actions on a self-hosted runner with CodeQL
SAST, runs as a non-root container with secrets in GCP Secret Manager, and a cron watchdog restarts stopped
containers and alerts on disk, CPU, and RAM.

`Python · Gemini / Vertex AI · ChromaDB · Docker · GitHub Actions · CodeQL · GCP Secret Manager`

### Incident-response playbook tool (RAG)
An event-driven pipeline over Kafka (Redpanda) that embeds incident-response playbooks into ChromaDB, clusters them
into MITRE-aligned threat categories, and has an LLM write one consolidated Master Playbook per cluster. It cut 500+
overlapping playbooks to 12, now in use across the SOC.

`Python · Kafka (Redpanda) · ChromaDB · LLM APIs`

## Personal projects

### [HomeSOC](https://github.com/galsakuri/HomeSOC)
Agent-based security monitoring for macOS. The agent collects process, file, network, and authentication events and
sends them to a FastAPI backend, where YAML detection rules raise alerts such as brute-force logins and outbound
connections to known C2 ports. Alerts go through a Redis queue to a live React/TypeScript dashboard over WebSocket.
Runs in Docker Compose, with pytest and GitHub Actions CI.

`Python · FastAPI · Redis · React · TypeScript · Docker Compose · GitHub Actions`

## Tech Stack

<p align="center">
  <img src="https://img.shields.io/badge/Splunk-000000?logo=splunk&logoColor=white"/>
  <img src="https://img.shields.io/badge/CrowdStrike-FC0000"/>
  <img src="https://img.shields.io/badge/MITRE%20ATT%26CK-B22222"/>
  <img src="https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white"/>
  <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?logo=githubactions&logoColor=white"/>
  <img src="https://img.shields.io/badge/GCP-4285F4?logo=googlecloud&logoColor=white"/>
  <img src="https://img.shields.io/badge/Gemini-8E75B2?logo=googlegemini&logoColor=white"/>
  <img src="https://img.shields.io/badge/ChromaDB-FF6446"/>
  <img src="https://img.shields.io/badge/Kafka-231F20?logo=apachekafka&logoColor=white"/>
  <img src="https://img.shields.io/badge/FastAPI-009688?logo=fastapi&logoColor=white"/>
  <img src="https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black"/>
  <img src="https://img.shields.io/badge/Git-F05032?logo=git&logoColor=white"/>
</p>

[LinkedIn](https://www.linkedin.com/in/gal-sakuri/)
