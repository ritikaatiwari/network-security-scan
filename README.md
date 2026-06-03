# Network Security Scan Project

## Objective

Perform a basic network reconnaissance scan using Nmap to identify open, closed, and filtered TCP ports on a target host.

## Tool Used

* Nmap 7.99

## Target
 
* scanme.nmap.org (45.33.32.156)

## Command Used

nmap scanme.nmap.org

## Scan Results

Open Ports:

* 22/tcp (SSH)
* 80/tcp (HTTP)
* 9929/tcp (Nping Echo)
* 31337/tcp (Elite)

Filtered Ports:

* 25/tcp (SMTP)
* 135/tcp (MSRPC)
* 139/tcp (NetBIOS Session Service)
* 179/tcp (BGP)
* 445/tcp (Microsoft-DS)
* 646/tcp (LDP)

## Analysis

The scan revealed several open services on the target host. Port 22 indicates that Secure Shell (SSH) is available for remote administration. Port 80 confirms that the host is serving web content over HTTP.

Several ports were marked as filtered, indicating that a firewall or network filtering device is preventing Nmap from determining whether the ports are open or closed. This demonstrates the use of defensive network controls to reduce service exposure.

The host responded successfully to scanning requests and was identified as online with low latency.

## Key Learnings

* Performed a TCP port scan using Nmap.
* Identified open, closed, and filtered ports.
* Learned basic service enumeration.
* Understood how firewalls affect scan results.
* Practiced documenting findings in a professional format.
