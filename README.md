# Python TCP Port Scanner

A simple TCP port scanner built with Python and tested in a Kali Linux lab environment. This project was developed to practice Python socket programming, network reconnaissance, and fundamental cybersecurity concepts.

## Overview

The Python TCP Port Scanner checks a target host for open TCP ports within a specified port range.

It uses Python's built-in `socket` library to attempt TCP connections and identifies ports that are accepting connections.

## Features

* Hostname and IPv4 address support
* TCP port scanning
* Detection of open ports
* Command-line argument handling
* Basic error and exception handling
* Tested in a Kali Linux environment

## Technologies Used

* Python 3
* Python Socket Library
* Kali Linux
* TCP/IP Networking

## Usage

Run the scanner from the terminal:

```bash
python3 port_scanner.py <ip-or-hostname>
```

Example:

```bash
python3 port_scanner.py 192.168.1.10
```

The current version scans TCP ports **50–84**.

## Example Output

```text
--------------------------------------------------
Scanning target: 192.168.1.10
Time started: 2026-10-02 12:30:00
--------------------------------------------------
Port 80 is open
Port 443 is open
```

## How It Works

1. The user provides an IP address or hostname.
2. The hostname is resolved to an IPv4 address if necessary.
3. The scanner creates a TCP socket for each port.
4. It attempts to establish a connection to the target port.
5. If the connection succeeds, the port is reported as open.
6. The socket is closed before scanning the next port.

## Learning Outcomes

This project helped me practice:

* Python socket programming
* TCP networking
* Port scanning concepts
* Network reconnaissance
* Command-line arguments
* Exception handling
* Basic cybersecurity enumeration

## Limitations

This is a basic educational port scanner and is not intended to replace professional network scanning tools such as Nmap.

Current limitations include:

* Scans only ports 50–84
* Performs TCP connection scanning
* Does not identify running services
* Does not perform banner grabbing
* Does not include advanced scanning techniques

## Future Improvements

Planned improvements may include:

* Custom port ranges
* Multithreaded scanning
* Service detection
* Banner grabbing
* Additional command-line options
* Scan result reporting

## Responsible Use

This tool should only be used against systems that you own or have explicit permission to test.

Unauthorized scanning of systems or networks may violate applicable laws, policies, or terms of service.

## Author

**Richmond Addo**

Cybersecurity Student | Python | Networking | Ethical Hacking

GitHub: [AddoRichmond-GH](https://github.com/AddoRichmond-GH)
