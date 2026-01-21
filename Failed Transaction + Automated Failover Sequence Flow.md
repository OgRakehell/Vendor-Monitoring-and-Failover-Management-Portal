## Failed Transaction + Automated Failover Sequence Flow
### Sequence Flow
 ### 1. Customer Initiates Transaction

- Customer requests airtime or data via an application channel.

### 2. Transaction Router Selects Vendor

- Routing logic selects Vendor A based on availability and priority.

### 3. API Call to Vendor A

- Transaction request is sent to Vendor A’s API.

### 4. Vendor Failure Occurs

- Vendor A responds with:

  - Timeout, error response, or repeated transaction failure.

### 5. Transaction Outcome Logged

- Failure is recorded with:

  - Vendor ID
  
  - Transaction type
  
  - Telco
  
  - Error response

- Metrics engine updates real-time failure counters.

### 6. Health Threshold Evaluation

- Failover engine evaluates Vendor A against predefined thresholds:

  - Failure rate
  
  - Consecutive failures
  
  - SLA breach indicators

### 7. Automated Vendor Deactivation

- Vendor A is marked as unhealthy

- Routing engine temporarily disables Vendor A

### 8. Traffic Rerouted

- Subsequent transactions are automatically routed to Vendor B

- No customer-facing interruption beyond the initial failure

### 9. Escalation Triggered

- Escalation workflow notifies Vendor A in real time

- Internal teams gain visibility via the portal

### 10. Portal Update

- Dashboard reflects:

  - Vendor A status: Disabled (Auto)
  
  - Failure trends
  
  - Failover activation timestamp

### Outcome:
Customer impact is minimized, operations remain stable, and recovery begins immediately.
