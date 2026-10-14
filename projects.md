---
layout: page
title: Projects
permalink: /projects/
---

# Projects

A mix of open-source work and production engineering. Customer-specific details are kept general to
respect confidentiality.

## Open source

<div class="project-card">
  <h3>FanDeck for Atomberg — macOS menu bar app</h3>
  <p>A native macOS menu bar app to control Atomberg smart ceiling fans (power, speed 1–6, and light)
  from the Mac, built on the official Atomberg Home public API.</p>
  <ul>
    <li><strong>Swift / SwiftUI</strong> menu bar app that builds with Command Line Tools alone — no full Xcode or Apple ID.</li>
    <li><strong>Quota-aware API client</strong>: token caching, batched reads, lazy polling, a command reserve, and 429 back-off.</li>
    <li><strong>Optimistic UI with delayed confirmation</strong> for the gap between a command being accepted and applied.</li>
    <li><strong>Secure by default</strong>: credentials in the macOS Keychain via the Security framework; ephemeral <code>URLSession</code>; no secrets on disk or in logs.</li>
    <li><strong>CI/CD</strong>: GitHub Actions builds and publishes a downloadable release on each tagged version.</li>
  </ul>
  <p class="project-tech">Swift · SwiftUI · Keychain / Security framework · URLSession · GitHub Actions</p>
  <a href="https://github.com/vmarpadge/fandeck-for-atomberg" class="btn btn-outline" target="_blank">View on GitHub →</a>
</div>

<div class="project-card">
  <h3>Parkinson's Detection Using Machine Learning</h3>
  <p>Detecting Parkinson's disease from sustained-vowel speech samples using signal features and an
  SVM classifier, with particle-swarm optimization for feature selection.</p>
  <ul>
    <li>Feature extraction (jitter, shimmer, HNR/NHR, pitch) from the UCI voice dataset.</li>
    <li>Dimensionality reduction via Particle Swarm Optimization (PSO).</li>
    <li>SVM classification for healthy-vs-affected prediction.</li>
  </ul>
  <p class="project-tech">Python · Machine Learning · SVM · PSO · signal processing</p>
  <a href="https://github.com/vmarpadge/Parkinsons-Detection-Using-Machine-Learning" class="btn btn-outline" target="_blank">View on GitHub →</a>
</div>

## Production engineering

<div class="project-card">
  <h3>Agentic &amp; GenAI solutions on Amazon Bedrock</h3>
  <p>Build and troubleshoot AI agents and MCP servers that connect large language models to tools and
  internal systems, deployed on Amazon Bedrock and Bedrock AgentCore for enterprise customers —
  including MCP integrations for observability and ticketing tools.</p>
  <p class="project-tech">Amazon Bedrock · Bedrock AgentCore · MCP · RAG / Knowledge Bases · Guardrails</p>
</div>

<div class="project-card">
  <h3>Internal diagnostic tooling for support engineers</h3>
  <p>A troubleshooting dashboard and automated issue detector (JavaScript/Node.js) that replaced
  manual, repetitive investigation steps across the team. Delivered from design doc and engineering
  review through implementation, with 98 unit tests at 95% coverage and documentation for handoff.
  An MCP interface so AI assistants can use the tool is planned next.</p>
  <p class="project-tech">Node.js · Jest · AWS SDK · code review · runbooks</p>
</div>

<div class="project-card">
  <h3>Reliability &amp; cost optimization at scale</h3>
  <p>Resolved complex production issues across 200+ deployments (ECS/EKS, Lambda, networking, CI/CD),
  and led customer recovery during a large-scale service event. Advised on Blue/Green and Canary
  release safety, helping customers reach ~40% lower cloud spend and 99.9% uptime; reproduced
  environments with Terraform, CloudFormation, and AWS CDK to isolate failures.</p>
  <p class="project-tech">ECS · EKS · Lambda · Terraform · CloudFormation · AWS CDK · CloudWatch</p>
</div>
