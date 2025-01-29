# Nonfunctional Testing with JMeter
### Test Server URL
[https://test460.nop-station.com/en/](https://test460.nop-station.com/en/)
### Tools
**JMeter 5.6.3**

## Supported Test Protocols in JMeter

### 1. HTTP Request
### 2. FTP (File Transfer Protocol)
- **Uploading files**
- **Downloading files**
- **Managing remote server files**
### 3. JDBC (Java Database Connectivity)
### 4. SMTP (Simple Mail Transfer Protocol)
### 5. SOAP API (Simple Object Access Protocol)
### 6. REST API (Representational State Transfer)
### 7. TCP (Transmission Control Protocol)
### 8. UDP (User Datagram Protocol)
### 9. JMS (Java Message Service)
### 10. DAP (Lightweight Directory Access Protocol)
### 11. SMTP, POP3, and IMAP

## Types of Load Tests

### 1. Performance/Load Test
- Evaluates application performance under expected user load.
- Measures response time, throughput, and resource utilization.

### 2. Soak/Endurance Test
- Tests system stability over an extended period under a typical or high load.
- Identifies memory leaks, performance degradation, and resource consumption.

### 3. Spike Test
- Assesses system behavior under sudden traffic surges.
- Ensures system can handle unexpected demand increases without failure.

### 4. Stress Test
- Determines system limits by pushing beyond expected capacity.
- Identifies breaking points and recovery mechanisms.

---

## Load Model in JMeter

### 1. Concurrency User
- Simulates multiple users interacting with the system simultaneously.
- Helps assess performance under varying loads.

### 2. Throughput
- Measures system requests processed per second.
- Evaluates scalability and performance.

### 3. Arrival Rate
- Defines how fast new requests arrive at the system.
- Simulates real-world user behavior.

---

## Structure of a Test Case in JMeter

### 1. Ramp-Up
- Gradually increases the number of virtual users.
- Prevents sudden load spikes.


### 2. Plateau/Step
- Sustains maximum load for a period to evaluate system performance.

### 3. Ramp-Down
- Gradually decreases load to simulate real-world scenarios.

---

## Visualization of Results with Listeners

### 1. View Results Tree
- Displays each request and response in a hierarchical format.
- Helps in debugging and error identification.

### 2. Summary Report
- Provides a tabular summary of test metrics:
  - **Number of requests**
  - **Average, min, and max response times**
  - **Error percentage**
  - **Throughput**

### 3. Aggregate Report
- Aggregates performance metrics for different requests.
- Useful for performance comparisons.

### 4. Graph Results
- Visualizes performance data, highlighting trends and spikes.

### 5. Response Time Graph
- Graphs response times to identify latency issues.

### 6. View Results in Table
- Displays results in a structured table format.

### 7. Simple Data Writer
- Exports test results to CSV or XML for further analysis.

### 8. JTL (JMeter Test Log)
- Stores detailed logs of each test execution.
- Can be analyzed with third-party tools.

---

## Project Workflow

### 1. Plan the Test
- Define objectives and testing parameters.

### 2. Decide on the Number of Users
- Determine concurrent users (e.g., 40 users for simulation).

### 3. Write and Run Test Cases
- Define test scenarios and execute tests.

### 4. Review the Test Report
- Analyze metrics like throughput, response time, and errors.

---

## Test Server Details

### Protocol & Configuration
- **Protocol:** HTTPS
- **Port:** 443
- **Server IP:** `test460.nop-station.com`
- **Path:** Defines the API endpoint being tested.




