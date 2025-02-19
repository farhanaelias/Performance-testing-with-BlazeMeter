# Performance Testing by using BlazeMeter

This repository contains a performance testing report for the North South University webpage (https://www.northsouth.edu/) 

This project involves performance testing using the BlazeMeter extension, JMeter, and command-line commands for report generation.

# Tools Used

BlazeMeter Extension: Used for recording and running performance tests.

JMeter: For detailed analysis of load testing scenarios.

Command-line commands: Used to execute JMeter tests and generate reports.

Google Chrome: Used to navigate and interact with the test site.

# Testing Process

Test Scenario Recording:

Recorded user interactions on the NSU site using the BlazeMeter extension.

Captured actions. 

Performance Test Execution:

Ran the recorded script through BlazeMeter.

Configured virtual users (VUs) to simulate multiple users accessing the site simultaneously.

Opened the file on JMeter

Used JMeter (Thread group) to conduct further load testing.

Executed JMeter tests via command-line commands and generated performance reports.

Constrains:

Number of Threads (users): 50

Ramp-Up Period (in seconds): 10

Loop Count: 1

# Make jtl file

  jmeter -n -t  NSU.jmx -l report\NSU.jtl

# Make html file

  jmeter -g report\NSU.jtl -o report\NSU.html 

# Metrics Collected:

Response time for each page.

Throughput (requests per second).

Error rate under load conditions.

Resource utilization and bottlenecks.

# Number of Threads 50 ; Ramp-Up Period 10s

![image](https://github.com/user-attachments/assets/c7c71070-9683-4723-b95e-c8c9cf5e4b51)


  
