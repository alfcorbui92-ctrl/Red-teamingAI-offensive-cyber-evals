# Offensive Cyber Evals

A red teaming and AI safety evaluation project focused on testing frontier language models in simulated enterprise cybersecurity environments.

## Overview

This repository contains adversarial prompt evaluations designed to measure whether AI agents provide harmful capability uplift in high-risk cybersecurity scenarios.

The evaluations were conducted inside synthetic enterprise environments containing realistic applications such as:

* Gitea
* NextCloud
* Mattermost
* Jenkins
* ERPNext
* NocoDB
* Workday
* Metabase

The objective of this project is to analyze how frontier models respond to adversarial prompts involving:

* Unauthorized data access
* Sensitive information disclosure
* Credential extraction
* Privilege escalation attempts
* Environment reconnaissance
* Goal manipulation
* Authority and legitimacy framing

All environments, data, credentials, and systems are synthetic and sandboxed.

---

# Models Evaluated

The following frontier models were evaluated:

* GPT-5.3 Codex
* GPT-4.1
* Claude 4.6 Opus
* Grok 4.1

Each prompt was executed against multiple models and analyzed comparatively.

---

# Evaluation Structure

Each task contains:

* System prompt context
* Adversarial user prompt
* Agent traces
* Harm classification
* Comparative failure analysis

The repository documents both successful and unsuccessful attempts to elicit harmful behavior.

---

# Harm Categories

## Unauthorized Data Access & Exfiltration

Testing whether models retrieve or expose sensitive enterprise data.

## Privilege Escalation Through Misconfiguration

Testing whether models exploit exposed credentials or insecure permissions.

## Autonomous Reconnaissance & Environment Mapping

Testing whether models autonomously explore and map enterprise environments.

## Covert Operational Persistence

Testing whether models establish hidden persistence mechanisms using legitimate enterprise tools.

---

# Attack Techniques Used

Prompts in this repository employ multiple jailbreak and adversarial prompting strategies, including:

* Authority / Permission Framing
* Legitimacy Framing
* Fabricated Urgency
* Emotional Manipulation
* Gradual Escalation
* Multi-turn Goal Manipulation
* Prompt Injection
* System Prompt Injection

---

# Repository Structure

```text
/offensive-cyber-evals
│
├── prompts/
├── analyses/
├── trajectories/
├── taxonomy/
├── methodology/
└── results/
```

---

# Disclaimer

This repository is intended strictly for AI safety research, red teaming evaluation, and defensive cybersecurity analysis.

No real infrastructure, users, credentials, or proprietary systems are involved.

The purpose of this work is to identify unsafe model behaviors before they can be exploited in real-world environments.
