# Vendor-Monitoring-and-Failover-Management-Portal
>Disclaimer

>This project models a real-life solution that I contributed to. To maintain confidentiality and security, all sensitive information, proprietary logic, vendor names, and specific architectural details have been changed or abstracted.

>This repository serves strictly as a demonstration of system design, product thinking, and operational logic, not a disclosure of any production system.

## Overview
This project models a real-world internal platform designed to manage airtime and data vendors in a high-volume transaction environment.

In the existing setup, the system relied on manual SQL updates to disable failing vendors whenever issues occurred. This approach had low visibility, was error-prone, reactive, and did not scale as transaction volume and vendor count increased.

The proposed solution introduces a centralized Vendor Management Portal that provides real-time visibility, automated failover, SLA tracking, and controlled intervention for authorized technical users.

This repository demonstrates the system design, business logic, and operational thinking behind the solution.

> I hope you find it interesting. Let us dive in!
