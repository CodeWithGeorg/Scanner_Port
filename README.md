# Scanner_Port
Multithreaded C++ TCP port scanner . Fast, small, for learning and authorized pentesting.

# Simple C++ Port Scanner

A lightweight, multithreaded TCP port scanner written in C++17.  
It performs non-blocking `connect()` calls with a timeout and supports scanning a port range concurrently using threads.

> **Warning:** Only scan systems you own or have explicit permission to test. Unauthorized scanning may be illegal.

## Features
- Hostname or IPv4 input
- Configurable port range (default 1–100)
- Multithreaded scanning (configurable number of threads)
- Non-blocking `connect()` with timeout (avoids long hangs)
- Simple output listing open ports

## Requirements
- Linux (Kali recommended)
- `g++` with C++17 support
- POSIX sockets (the code uses POSIX APIs)

On Kali install build tools:

```bash
sudo apt update
sudo apt install -y build-essential
