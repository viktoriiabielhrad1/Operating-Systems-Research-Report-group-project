Operating Systems Research Report
-
COMPH1037 — Operating Systems
Group Members: Viktoriia Bielhrad, Valentina Pruteanu, Rysean Dyle Soy, Angelo Bundac

This project investigates how Microsoft Edge interacts with the Windows operating system through 
its multi‑process architecture. The report analyses memory usage, performance behaviour, process
management, network activity, crash recovery, security features, and sandbox isolation.

Performance & Memory Management
-
The report examines Edge’s use of RAM, preloading and prediction processes, virtual memory (pagefile.sys),
committed memory, and background updates via Task Scheduler. It explains paging, page faults, and how Edge 
allocates memory dynamically depending on tabs, content, and extensions.

Process Management
-
The main browser process, renderer process, and GPU process are analysed using Task Manager,
Edge Task Manager, Process Explorer, and Resource Monitor. Tests include single‑tab and multi‑tab
behaviour, video playback at different resolutions, context switches, thread activity, and inactive tab suspension.

Network Process
-
Using Wireshark, the report evaluates DNS queries, bandwidth usage, and network load under 
different video resolutions and multiple tabs. Results show significant increases in network 
activity with higher workloads and streaming quality.

Crash Handler
-
Crashpad‑handler behaviour is tested using controlled browser crashes. CPU usage and recovery 
time are measured for single‑tab and multi‑tab scenarios, showing how recovery scales with workload.

SmartScreen & Tracking Protection
-
The report analyses SmartScreen’s role in blocking malicious sites and downloads. CPU usage, 
thread activity, and performance impact are measured using Process Explorer and Edge DevTools.

Sandbox Process
-
Windows Sandbox is evaluated as an isolated environment for testing untrusted software. 
Differences in CPU and memory usage between the real system and sandbox are documented.

Third‑Party & Extension Processes
-
The report explains how Edge handles third‑party components and browser extensions, 
including Intune‑based extension control. It discusses how extensions affect CPU and memory 
usage and outlines best practices for reducing resource consumption.

Conclusion
-
The project provides a detailed exploration of Edge’s architecture and its interaction with 
system resources. It highlights how processes, memory management, network activity, and security 
mechanisms contribute to performance, stability, and safety.
