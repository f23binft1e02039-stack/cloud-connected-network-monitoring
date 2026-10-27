# Final Year Project Proposal

## 1. Project Title

**Design and Implementation of a Cloud-Connected Network Monitoring and Rule-Based Fault Diagnosis System for Multi-Site Networks**

## 2. Introduction

Modern organizations often operate across multiple branch offices, each depending on network connectivity and essential IT services. Monitoring these distributed environments is important for identifying service disruptions, reducing troubleshooting time, and maintaining operational availability.

Traditional manual monitoring can make it difficult to obtain a unified view of network health, identify the likely cause of a failure, and maintain a record of incidents and their recovery. A centralized monitoring system can help address these challenges by periodically checking network connectivity and service availability and presenting the results through a unified dashboard.

This project proposes the design and implementation of a cloud-connected network monitoring and rule-based fault diagnosis system for simulated multi-site networks. The system will monitor configured network endpoints and services, detect failures, collect diagnostic evidence, generate alerts, and maintain an incident history through a centralized web interface.

## 3. Problem Statement

Organizations operating multiple branch networks require timely information about network connectivity and the availability of critical services. Without centralized monitoring and systematic diagnostic records, identifying the location and likely cause of a disruption may require repeated manual checks, increasing troubleshooting effort and delaying fault resolution.

A monitoring system that combines periodic connectivity checks, service availability monitoring, evidence-based fault classification, and incident tracking could provide a more structured approach to network troubleshooting.

The problem addressed by this project is the lack of an integrated, accessible monitoring and diagnostic solution within the proposed simulated multi-site environment that can identify connectivity and service failures, record supporting evidence, and track incidents through recovery.

## 4. Project Aim

To design and implement a centralized network monitoring system that monitors simulated multi-site networks, detects connectivity and service failures, provides rule-based diagnostic information, and tracks incidents and service recovery through a web dashboard.

## 5. Project Objectives

1. To design a centralized architecture for monitoring multiple simulated branch networks and their associated services.
2. To implement periodic connectivity and service availability checks using appropriate network monitoring techniques.
3. To detect and classify common failures, including endpoint unreachability and application service unavailability.
4. To develop a rule-based fault diagnosis mechanism that uses monitoring results to generate likely diagnoses and record supporting evidence.
5. To develop a web dashboard displaying branch health, endpoint status, active alerts, incident history, and recovery information.
6. To maintain a database of monitoring results, diagnostic evidence, and incident lifecycle events.
7. To evaluate the system under controlled failure scenarios using metrics such as detection latency, fault classification accuracy, and recovery tracking performance.

## 6. Proposed Scope

The initial implementation will focus on a simulated multi-site environment consisting of a small number of virtual branches and configured network endpoints or services.

The system will include:

- Centralized monitoring of simulated branch endpoints.
- Periodic HTTP and TCP service checks, with ICMP-based reachability checks where supported.
- Detection of endpoint and service failures.
- Rule-based diagnosis using available monitoring evidence.
- Dashboard-based status visualization and alert presentation.
- Incident creation, event history, and recovery tracking.
- Controlled testing of normal operation, connectivity failures, service failures, and service restoration.

The initial system will run in a local development environment. Cloud deployment may be included as an extension if time and resources permit.

The project will not initially target production-scale enterprise monitoring, automated network configuration changes, advanced machine-learning diagnosis, or guaranteed monitoring of geographically distributed physical networks.

## 7. Proposed Methodology

The project will follow an iterative design, implementation, and testing approach.

**Phase 1: Requirements and system design**

Identify monitoring requirements, define representative branch scenarios, specify failure conditions, and design the application architecture and database.

**Phase 2: Monitoring engine development**

Implement scheduled connectivity and service checks, collect check results, and determine endpoint health using predefined status rules.

**Phase 3: Fault diagnosis and incident management**

Develop rules for interpreting monitoring results, recording diagnostic evidence, generating alerts, and tracking incidents from detection through recovery.

**Phase 4: Dashboard and database integration**

Develop the web interface and integrate it with the backend API and database to display network status, monitoring history, and incident information.

**Phase 5: Testing and evaluation**

Introduce controlled failures into the simulated environment, verify the resulting system behaviour, measure performance, and document the findings.

## 8. Proposed Technologies

- **Programming language:** Python
- **Backend framework:** FastAPI
- **Frontend:** HTML, CSS, and JavaScript
- **Database:** SQLite
- **Network monitoring:** HTTP, TCP, and supported ICMP connectivity checks
- **Testing:** Controlled endpoint and service failure scenarios
- **Development environment:** Windows-based local environment
- **Optional extension:** Deployment to a cloud-hosted virtual machine

## 9. Expected Outcomes

The project is expected to produce:

1. A functional centralized network monitoring application for simulated multi-site networks.
2. A web dashboard providing a consolidated view of branch and service health.
3. A monitoring engine capable of detecting configured connectivity and service failures.
4. A rule-based diagnostic component that records likely fault categories and their supporting evidence.
5. An incident management mechanism that records detection, status changes, and service recovery.
6. An evaluation report containing measured detection latency, fault classification results, and recovery tracking observations.
7. Technical documentation covering system architecture, implementation, testing, limitations, and possible future improvements.

## 10. Significance of the Project

The project will demonstrate the application of networking concepts, service monitoring, backend development, database management, and web-based visualization to a practical IT operations problem.

By combining monitoring results with diagnostic evidence and incident history, the proposed system aims to provide a structured and testable approach to troubleshooting within a simulated multi-site environment. The evaluation will help establish its effectiveness and identify limitations under the selected test scenarios.

## 11. Deliverables

- Project requirements and system design documentation.
- System architecture and database design.
- Functional monitoring engine and backend API.
- Centralized web dashboard.
- Rule-based fault diagnosis and incident tracking.
- Controlled test scenarios and evaluation results.
- Final project report and demonstration.

## 12. Conclusion

This project proposes a practical network monitoring and fault diagnosis solution that combines centralized visibility, automated service checks, evidence-based fault classification, and incident recovery tracking. The resulting application will provide a working demonstration of networking and software engineering concepts while offering measurable outcomes for academic evaluation.
