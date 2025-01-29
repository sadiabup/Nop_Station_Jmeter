# Non functional Testing with JMeter
## Overview
JMeter is an open-source tool designed for performance and load testing of web applications, APIs, and other services. This guide details the step-by-step installation process of Java JDK, Maven, and JMeter, followed by an in-depth exploration of JMeter's testing capabilities. It covers different test types, load models, and result analysis techniques to help users optimize system performance.

### Test Server URL
[https://test460.nop-station.com/en/](https://test460.nop-station.com/en/)

### Tools
- Java JDK 23.0.1
- Maven 3.9.9
- JMeter 5.6.3

## 1. Installation Process:

### Java JDK Installation
1. Visit: [Oracle Java Download](https://www.oracle.com/bd/java/technologies/downloads/)
2. Choose **JDK 23** and select **x64 Installer** for Windows.
3. Extract the downloaded file and move it to a desired directory.
4. Copy the path up to the `bin` folder and save it as a **System Environment Variable**.
5. Verify installation by running the following command in the terminal:
   ```sh
   java --version
   ```

### Apache Maven Installation
1. Visit: [Maven Download](https://maven.apache.org/download.cgi)
2. Choose **Binary zip archive** from the list.
3. Extract the downloaded file.
4. Copy the path up to the `bin` folder and save it as a **System Environment Variable**.
5. Verify installation by running the following command in the terminal:
   ```sh
   mvn --version
   ```

### JMeter Installation
1. Visit: [JMeter Download](https://jmeter.apache.org/download_jmeter.cgi)
2. Choose the **zip file** from the binaries.
3. Extract the downloaded file.
4. Copy the path up to the `bin` folder and save it as a **System Environment Variable**.
5. Verify installation by running the following command in the terminal:
   ```sh
   jmeter -v
   ```

---


## Supported Test Protocols in JMeter

#### 1. HTTP Request
#### 2. FTP (File Transfer Protocol)
- **Uploading files**
- **Downloading files**
- **Managing remote server files**
#### 3. JDBC (Java Database Connectivity)
#### 4. SMTP (Simple Mail Transfer Protocol)
#### 5. SOAP API (Simple Object Access Protocol)
#### 6. REST API (Representational State Transfer)
#### 7. TCP (Transmission Control Protocol)
#### 8. UDP (User Datagram Protocol)
#### 9. JMS (Java Message Service)
#### 10. DAP (Lightweight Directory Access Protocol)
#### 11. SMTP, POP3, and IMAP

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


##  Creating a JMeter Test Project

### 1. Plan the Test
- Define objectives and expected system behavior.

### 2. Configure Users
- Decide the number of users to simulate (e.g., 10 users).

### 3. Write and Execute Test Cases
- Implement test scripts and execute them to simulate real traffic.

![Image](https://github.com/user-attachments/assets/d2b3fbcb-0546-47b4-8d49-ce4428671758)

### 4. Analyze Test Reports
- Examine key performance metrics such as:
  - **Throughput** (data processed per second)
  - **Response time**
  - **Error rates**
  - **System stability**

    ![Image](https://github.com/user-attachments/assets/923484f8-4ad3-429c-a192-6f06e1c56705)


![Image](https://github.com/user-attachments/assets/9c2e6346-b616-4810-b032-9ea3edbdd328)


![Image](https://github.com/user-attachments/assets/728c5aa1-1458-4a94-ace8-97a7f366a9d3)

---

## Test Server Details

### Protocol & Configuration
- **Protocol:** HTTPS
- **Port:** 443
- **Server IP:** `test460.nop-station.com`
- **Path:** Defines the API endpoint being tested.

---

##  References
- Mentor: Md. Al Foysal Rabbi
  - **SQA Engineer**
  - **Brain Station 23**
  - ![LinkedIn Logo](https://upload.wikimedia.org/wikipedia/commons/c/ca/LinkedIn_logo_initials.png) 



