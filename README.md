# Wireshark Traffic Analysis 2

This repository contains Wireshark `.pcapng` capture files and a corresponding analysis report for educational purposes. It demonstrates how to use Wireshark to analyze HTTP traffic and extract useful information such as:

- HTTP version used by the browser
- Local IP address of the client
- Server IP address (e.g., gaia.cs.umass.edu)
- Frame numbers of GET requests and responses
- Number of GET requests sent
- Server response codes and content sizes
- Serial vs. parallel image fetching behavior
- Authorization headers and response status (401 Unauthorized, etc.)

## Files Included

- `capture-1.pcapng`
- `capture-2.pcapng`
- `capture-3.pcapng`
- `capture-4.pcapng`
- `NursenaTaskopru2.pdf` — Detailed written analysis in Turkish by Nursena Taşköprü

## Author

- Nursena Taşköprü
2024–2025 Spring — Computer Networks

## Usage

To explore the traffic captures yourself:

1. Open `.pcapng` files in Wireshark.
2. Use filters like:
   - `http.request`
   - `http.response`
   - `http.request.method == "GET"`
   - `arp || dhcp`
3. Check timestamps, IPs, status codes, and content lengths.

