---
children_hash: 8c924201461f9be75a17e7872392e5fda10af0e4923e18d49e15f05acd881545
compression_ratio: 0.7041284403669725
condensation_order: 1
covers: [portfolio_automation.md, vibe_advertising_pipeline.md, vibe_advertising_pipeline/_index.md]
covers_token_total: 872
summary_level: d1
token_count: 614
type: summary
---
# Portfolio and Advertising Automation Overview

This domain consolidates automation strategies for portfolio management and high-performance advertising asset generation. It is anchored by two primary initiatives: the core Portfolio Automation framework and the specialized Vibe Advertising Pipeline.

## Portfolio Automation
Documented in [portfolio_automation.md](portfolio_automation.md), this project focuses on the infrastructure for a Next.js-based portfolio. 
* Key Architecture: Integration with Medusa.js and WooCommerce to manage product and content flows.
* Core Functionality: Automates blog updates and repository synchronization via GitHub.

## Vibe Advertising Pipeline
The Vibe Advertising Pipeline represents a sophisticated "Content Engine 2.0" designed for rapid asset generation and cross-platform distribution. Detailed in [vibe_advertising_pipeline.md](vibe_advertising_pipeline.md) and summarized in [vibe_advertising_pipeline/_index.md](vibe_advertising_pipeline/_index.md), this system replaces manual workflows with autonomous research and execution.

### Operational Workflow
The pipeline follows a 7-stage process:
1. Trend/Competitor Analysis: Automated scraping via OpenClaw.
2. Asset Ingestion: Processing of product media and technical documentation.
3. Strategic Matrix Generation: Utilizing Gemini Batch to produce 30-40 hooks categorized by awareness level (Cold, Problem, Solution, Product).
4. Selection Loop: User-driven approval of generated assets.
5. Multi-Model Generation: Orchestration using NanoBanana (static UGC/lifestyle) and Replicate (dynamic video).
6. Platform Adaptation: Tailored distribution for X, LinkedIn, and blogs.
7. Cloud Delivery: Automated archival to `/output/falko-project/`.

### Architectural Decisions
* Tooling Shift: Migration from Claude Co-work to OpenClaw and Playwright for autonomous research and distribution.
* Cost Optimization: Implementation of Gemini Batch for script/hook generation, reducing operational costs by ~50%.
* Automation Framework: Centralized orchestration using Playwright, NanoBanana, and xurl to maintain a continuous content lifecycle.

### Key Dependencies and Rules
* Core Dependencies: Gemini API, NanoBanana, xurl, and Playwright.
* Rules: Content must be generated across all defined awareness levels to ensure comprehensive audience reach.
* Governance: Refer to `SKILL_VIBE_PIPELINE.md` for specific skill definitions and implementation standards.