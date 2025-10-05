# DEMO
https://github.com/user-attachments/assets/29f05a3b-2a99-44ec-940b-2b6e39f68402


<img width="813" height="468" alt="image" src="https://github.com/user-attachments/assets/ae44b6b3-2f6e-4bf2-a8c6-d49ad6aff6d3" />


# InstaVibe: Multi-Agent AI System

A production-ready demonstration of enterprise multi-agent orchestration using Google's Agent Development Kit (ADK), Agent-to-Agent (A2A) protocol, and Model Context Protocol (MCP).

---

## Overview

InstaVibe is a social platform enhanced with an intelligent event planning assistant that leverages multiple specialized AI agents to analyze user profiles, generate personalized recommendations, and automatically create social events.

---

## Architecture

The system implements a distributed multi-agent architecture with four specialized agents:

### Specialized Agents
- **Social Profiling Agent**: Analyzes user relationships, posts, and event history using Spanner Graph Database.
- **Event Planner Agent**: Generates creative, location-specific event suggestions with real-time Google Search integration.
- **Platform Interaction Agent**: Interfaces with InstaVibe APIs through MCP server to create posts and events.
- **Orchestrator Agent**: Central coordinator deployed on Vertex AI Agent Engine that delegates tasks via A2A protocol.

### Technology Stack
- **Framework**: Google Agent Development Kit (ADK)
- **Protocols**: A2A (agent communication), MCP (tool integration)
- **Database**: Google Cloud Spanner with Graph capabilities
- **Deployment**: Google Cloud Run (agents), Vertex AI Agent Engine (orchestrator)
- **Observability**: Cloud Trace for performance analysis

---

## Key Features

- Graph-based social analysis with multi-hop relationship queries
- Real-time event recommendations grounded in web search results
- Stateful agent workflows with loop agents and callbacks
- Distributed agent orchestration with standardized protocols
- Production-ready deployment on managed Google Cloud services

---

## System Flow

1. User submits event planning request with friends, date, and location.
2. Orchestrator delegates to Social Agent for profile analysis.
3. Social Agent queries graph database for interests and relationships.
4. Orchestrator sends findings to Planner Agent for recommendations.
5. Planner performs web searches and generates tailored suggestions.
6. User confirms plan.
7. Orchestrator delegates to Platform Agent to create post/event via MCP.
8. Event appears on InstaVibe platform.

---


---

## Technical Highlights

- Multi-agent coordination with sequential and loop workflows
- State management for cross-iteration data persistence
- Custom callbacks for lifecycle event handling
- Remote agent discovery via Agent Cards
- Standardized tool integration with MCP servers
- Cloud-native scalability with independent service deployment

---

## Performance

- Average end-to-end planning: 90-120 seconds
- Concurrent agent execution via A2A
- Cloud Trace integration for latency analysis
- Optimized with managed service infrastructure

---

## Prerequisites

- Google Cloud Project with billing enabled
- Cloud Spanner instance with Graph support
- Vertex AI API enabled
- Cloud Run and Agent Engine permissions

---

## Deployment

All agents deployed as containerized services:

- Specialized agents on Cloud Run
- Orchestrator on Vertex AI Agent Engine
- MCP server on Cloud Run
- InstaVibe web app on Cloud Run

---

## Use Cases

- **Event Planning**: Automated social event creation with personalized recommendations
- **Customer Service**: Multi-agent workflows for complex support scenarios
- **Workflow Automation**: Distributed task orchestration across specialized agents
- **Knowledge Synthesis**: Combining multiple data sources for intelligent insights



