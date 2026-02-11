---
title: "Project Resources"
date: 2026-02-11
categories: ["tools"]
tags: ["resources", "repositories", "IoT", "AI", "bird-detection"]
summary: "A central directory of all project repositories, with descriptions and links to get started."
draft: false
---

## Project Resources & Repositories

This page serves as a central hub for all the repositories and resources related to our AI‑powered backyard bird monitoring and home defence ecosystem. Whether you're looking for the edge detection software, the MQTT messaging layer, the agentic blog engine, or the project website itself, you'll find it here.

---

### 🐦 BirdLense

**Smart bird feeder system** — A Raspberry Pi‑powered smart bird feeder that uses computer vision and audio recognition to detect, identify, record, and analyse birds. Built with Python, React, and runs entirely on your local network using Docker.

- Two‑stage detection: YOLO bird detector + species classifier
- BirdNET audio identification
- Optional LLM verification (Google Gemini) for low‑confidence detections
- Species visit tracking, daily AI summaries, and timeline video playback
- Push notifications via ntfy and MQTT
- MCP (Model Context Protocol) support for AI agent integrations

🔗 [github.com/toddwhitehead/BirdLense](https://github.com/toddwhitehead/BirdLense)

---

### 🎯 birdwatch‑ai

**Hybrid AI bird identification** — A hybrid neural detection system for real‑time bird identification running on Raspberry Pi 5 with Hailo‑8 NPU acceleration. Combines visual detection (YOLOv8 + TensorFlow Lite classification) with audio recognition (BirdNET) for cross‑referenced species identification.

- Hailo‑8 NPU object detection at 33 ms per frame
- TFLite species classifier covering 965 bird species
- BirdNET audio analysis with location‑aware filtering
- Flask web dashboard with live stats and Server‑Sent Events
- IP camera RTSP integration

🔗 [github.com/toddwhitehead/birdwatch-ai](https://github.com/toddwhitehead/birdwatch-ai)

---

### 📡 acme‑mqtt

**Azure Event Grid MQTT Integration** — A Docker‑based MQTT solution that bridges on‑premises MQTT infrastructure with Azure Event Grid's MQTT broker. Messages from local IoT devices flow through a local Mosquitto broker, get augmented with metadata by a proxy service, and are forwarded to Azure Event Grid for cloud processing and storage.

- Local Eclipse Mosquitto MQTT broker
- Python MQTT proxy with message enrichment (timestamps, metadata)
- Azure Event Grid MQTT broker integration (TLS on port 8883)
- Azure Function for routing events to Blob Storage
- Infrastructure as Code with Bicep templates and deployment scripts

🔗 [github.com/toddwhitehead/acme-mqtt](https://github.com/toddwhitehead/acme-mqtt)

---

### ✍️ Agentic Blog Bird

**Multi‑agent blog generator** — A multi‑agent system for automatically generating entertaining blog posts from bird detection event data and telemetry. Built with Microsoft Agent Framework on Azure AI Foundry.

- Six specialised agents: Editor, Researcher, CopyWriter, Artist, Publisher, and Committer
- Reads bird detection data from Azure Blob Storage
- Generates cartoon‑style images inspired by Wile E. Coyote and Road Runner
- Outputs Hugo‑compatible markdown with front matter
- Auto‑commits posts to Azure DevOps Git

🔗 [github.com/toddwhitehead/agentic-blog-bird](https://github.com/toddwhitehead/agentic-blog-bird)

---

### 🌐 acme‑giyt‑web

**Project website** — The Hugo static site you're reading right now. Contains blog posts, leadership frameworks, and project documentation. Deployed via GitHub Actions.

- Hugo static site generator
- CI/CD with GitHub Actions
- Markdown‑driven content

🔗 [github.com/toddwhitehead/acme-giyt-web](https://github.com/toddwhitehead/acme-giyt-web)

---

### 📸 acme‑twirly

**WiFi‑controlled photography turntable** — A Raspberry Pi Pico W‑controlled precision turntable for product photography, 360° documentation, and time‑lapse videos. Uses a DRV8825 stepper motor driver with 3D‑printed gears.

- Microstepping control (1–32 microstepping) for smooth rotation
- Mobile‑friendly web interface with dark mode
- Timelapse mode for automated photography sequences
- mDNS network access (http://picow.local)

🔗 [github.com/toddwhitehead/acme-twirly](https://github.com/toddwhitehead/acme-twirly)

---

## Microsoft AI & Agent Resources

Key Microsoft platforms and frameworks used across these projects.

### Microsoft Foundry (Azure AI Foundry)

The agent factory — design, customise, manage, and support AI applications and agents at scale. Foundry provides access to models, agent orchestration, evaluation tools, and responsible AI capabilities.

- [Microsoft Foundry Documentation](https://learn.microsoft.com/en-us/azure/ai-foundry/)
- [Microsoft Foundry Portal](https://ai.azure.com/)
- [Quickstart — Create Foundry Resources](https://learn.microsoft.com/en-us/azure/ai-foundry/tutorials/quickstart-create-foundry-resources?view=foundry)
- [Foundry Agent Service — Build & Host AI Agents](https://learn.microsoft.com/en-us/azure/ai-services/agents/overview?view=foundry-classic)
- [Foundry SDKs (Python, C#, JavaScript, Java)](https://learn.microsoft.com/en-us/azure/ai-foundry/how-to/develop/sdk-overview?view=foundry-classic)

### Foundry Local

Run LLMs on your own device for free. Foundry Local automatically selects the best model variant for your hardware (NVIDIA GPU, AMD GPU, NPU, Apple Silicon, or CPU).

- [Get Started with Foundry Local](https://learn.microsoft.com/en-us/azure/ai-foundry/foundry-local/get-started?view=foundry-classic)
- [Integrate Inference SDKs with Foundry Local](https://learn.microsoft.com/en-us/azure/ai-foundry/foundry-local/how-to/how-to-integrate-with-inference-sdks?view=foundry-classic)
- [Compile Hugging Face Models for Foundry Local](https://learn.microsoft.com/en-us/azure/ai-foundry/foundry-local/how-to/how-to-compile-hugging-face-models?view=foundry-classic)
- [Foundry Local GitHub Repository](https://aka.ms/foundry-local-installer)

### Microsoft Agent Framework

Build robust, future-proof agentic AI solutions. The Agent Framework provides patterns for multi-agent orchestration, tool use, and workflow automation.

- [Agent Framework Documentation](https://learn.microsoft.com/en-us/agent-framework/)
- [Agent Framework Quick-Start Guide](https://learn.microsoft.com/en-us/agent-framework/tutorials/quick-start)
- [Python Samples](https://github.com/microsoft/agent-framework/tree/main/python/samples)
- [C# Samples](https://github.com/microsoft/agent-framework/tree/main/dotnet/samples)
- [Migrate from AutoGen to Agent Framework](https://learn.microsoft.com/en-us/agent-framework/migration-guide/from-autogen/index)
- [Migrate from Semantic Kernel to Agent Framework](https://learn.microsoft.com/en-us/agent-framework/migration-guide/from-semantic-kernel/index)
