# IT Systems and Services Management

**Network Design · Service Configuration · Perimeter Security · Infrastructure Monitoring**

Practical coursework combining **Cisco Packet Tracer** network simulations with virtualized **Debian** environments. The labs cover network connectivity, DNS and HTTP services, security with IPCop and a DMZ, and server monitoring with Nagios 4 and NCPA.

## Overview

This project documents the networking, security, and monitoring activities completed for **Unit 01: Security Management and Regulations** of the IT Systems and Services Management course.

The work connects networking fundamentals with practical administration: designing topologies, configuring services, checking connectivity, and diagnosing failures through system metrics and service checks.

## Technical Stack

| Technology | Role in the labs |
| --- | --- |
| **Cisco Packet Tracer** | Network design, device configuration, and traffic simulation |
| **Debian GNU/Linux** | Server administration and network diagnostics |
| **IPCop** | Firewall configuration and network security zones |
| **Apache HTTP Server** | Web service and Nagios web interface |
| **Nagios 4** | Centralized host and service monitoring |
| **NCPA** | Remote CPU, memory, and disk metrics |
| **UTM / VirtualBox** | Virtual machines for the lab environments |

## Featured Labs

### 01 · Network Design with Cisco Packet Tracer

Designed and configured topologies with routers, switches, wireless access points, clients, and servers to explore communication across multiple networks.

- Configured IPv4 addresses, subnet masks, and default gateways.
- Set up wired and wireless networks, including WPA2-PSK authentication.
- Configured DNS resolution and HTTP access from client devices.
- Applied NAT and port forwarding to private network scenarios.
- Examined the message exchanges involved in accessing a web service.

**Core concepts:** OSI and TCP/IP models, public and private addressing, ports, routing, DNS, HTTP, and NAT.

![Cisco Packet Tracer workspace showing routers connecting client networks to DNS and HTTP servers](docs/images/packet-tracer-topology.png)

*Network topology from the Packet Tracer lab, connecting client networks to DNS and HTTP services.*

### 02 · Perimeter Security with IPCop and a DMZ

Worked with a lab topology containing an IPCop firewall, an internal network, and a demilitarized zone (DMZ) for a Debian web server.

- Configured separate network zones for internal systems and the web server.
- Checked network connectivity and HTTP access.
- Explored the role of a DMZ in separating exposed services from an internal network.

<p align="center">
  <img src="docs/images/ipcop-dmz-architecture.png" alt="IPCop reference diagram showing external connectivity, an internal LAN, and a DMZ containing a Debian web server" width="520">
</p>

*Reference architecture from the lab brief, showing the IPCop firewall and its external, internal LAN, and DMZ zones.*

### 03 · Debian Server Monitoring with Nagios and NCPA

Configured a Nagios 4 server to monitor a second Debian machine, using NCPA to retrieve system resource metrics.

| Check | Purpose |
| --- | --- |
| **Host availability** | Verify that the monitored machine is reachable |
| **HTTP** | Check whether the web service responds |
| **CPU** | Track processor utilization |
| **Memory** | Track RAM utilization |
| **Disk** | Track storage utilization |

Configured `WARNING` and `CRITICAL` thresholds, validated Nagios configuration, and tested plugin execution under the Nagios service account.

**Documented outcome:** the monitored host was reachable, and its HTTP, CPU, memory, and disk checks reached an `OK` state. The final Nagios configuration validation reported zero errors.

![Nagios service dashboard showing OK states for the Debian server's HTTP, CPU, memory, and disk checks](docs/images/nagios-service-dashboard.png)

*Captured Nagios dashboard showing the Debian server's HTTP, CPU, memory, and disk checks in an OK state.*

## Troubleshooting and Validation

The monitoring lab included diagnosing and resolving:

- Connectivity failures caused by virtual machines being on different networks.
- Apache CGI configuration issues affecting the Nagios interface.
- Python interpreter and NCPA plugin execution issues.
- Missing Nagios command definitions and execution permissions.
- An incorrect NCPA disk metric path.

**Diagnostic tools:** `ip`, `ping`, `curl`, `nc`, `ss`, and `systemctl`.

## Skills Demonstrated

- Designing and validating network topologies in Cisco Packet Tracer.
- Configuring and verifying DNS and HTTP services.
- Working with NAT, firewall zones, and DMZ architectures.
- Monitoring Linux hosts, services, and resource utilization.
- Using diagnostic evidence to identify and resolve configuration issues.
- Documenting procedures, incidents, and verified results.

---

*Academic project completed in simulated and virtualized lab environments.*
