🧠 Lab Summary — NETSTAT
🎯 Objective

Learn how to use the Netstat command-line tool to monitor network connections, identify listening ports, analyze active sessions, and troubleshoot or detect suspicious network activity.

⚙️ Step-by-Step Overview

Introduction to Netstat

Understand that Netstat displays active network connections, routing tables, interface stats, and open ports.

Basic command:

netstat


Shows protocol, local/foreign address, and connection state.

Display Listening Ports

Identify services currently listening for incoming connections:

netstat -an | findstr LISTEN


Helps detect unauthorized or unexpected open ports.

Filter by Protocol

Focus on specific traffic types for analysis:

netstat -p tcp
netstat -p udp


View Network Statistics

Review network interface performance, bytes sent/received, and errors:

netstat -e


Show Connections by Application

Identify which applications or processes own active connections:

netstat -b


Advanced Combined View

Combine multiple flags for a complete overview:

netstat -ano


Explanation:

-a: Show all connections and listening ports.

-n: Display numeric addresses/ports.

-o: Show process ID (PID) per connection.

Real-World Application

Security monitoring: Detect unauthorized services.

Troubleshooting: Identify stalled or broken connections.

Incident response: Correlate suspicious processes with network activity.

🧩 Key Learning Points

Gain visibility into live network activity.

Detect anomalies or possible intrusions using Netstat.

Correlate open ports and connections with running processes for better security control.
