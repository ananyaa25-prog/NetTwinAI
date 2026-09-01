# Simulation Specification

## 1. Purpose

The NetTwinAI simulation represents a dynamic computer network in which network traffic, topology, routing conditions, and resource utilization change over time.

The simulator will generate different network conditions and measure their impact on service performance.

The generated simulation data will be used to develop and evaluate an **Explainable Digital Twin Framework for Predictive Network Service Degradation**.

The primary objective is to move network management from a reactive approach, where degradation is detected after it occurs, towards a predictive approach that identifies potential degradation before significant service impact occurs.

The simulation will support:

- Network state generation
- Dynamic traffic conditions
- Network service degradation
- Machine Learning-based prediction
- Explainable AI-based analysis
- Preventive action recommendation
- Digital Twin-based action evaluation

---

## 2. Network Environment

The simulated environment consists of multiple interconnected network devices and end hosts.

Initial development configuration:

- Number of routers: 4
- Number of end hosts: 6
- Number of communication links: Multiple
- Multiple possible paths between selected source and destination nodes
- Variable link bandwidth
- Dynamic network traffic

The network topology may be expanded during development.

Each network link has finite bandwidth and may experience changing utilization and congestion.

---

## 3. Network Topology Model

The network consists of:

- Routers
- End hosts
- Communication links
- Source-destination pairs
- Alternative routing paths

Example topology:

```text
             ┌─────────────┐
             │   Router 2  │
             └──────┬──────┘
                    │
                    │
┌─────────┐   ┌────┴──────┐   ┌─────────┐
│  Host A │───│  Router 1 │───│ Router 4│─── Host B
└─────────┘   └────┬───────┘   └────┬────┘
                    │                │
                    │                │
             ┌──────┴──────┐         │
             │   Router 3  │─────────┘
             └─────────────┘
