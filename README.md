# Lupo — Malware IOC Extractor
Debugging module for Malware Analysis Automation
## Introduction
Working on security incidents that involve malware, we come across situations on a regular basis where we feel the need to automate parts of the analysis process as complete manual analysis is, more often than not, not possible for every case due to many factors (time, skills, scale etc.).

I wrote Lupo mainly to automate and accelerate the process as much as possible. Lupo is a dynamic analysis tool that can be used as a module with the debugger. The first version works with the popular Windows Debugger — WinDbg. I’ll release versions for other debuggers in the future.

The way the tool works is pretty straight forward. You load Lupo into the debugger and then execute it. It runs through the malware and collects predefined IOC and writes them to a text file on the disk. You can then use this information to contain and neutralise malware campaigns or simply respond to the security incident that you are working on.

## Lupo — the tool
I’ll give some more details on the tool itself but not too much to the inner workings of it, at least not here. We need to keep in mind that the malware authors are smart enough to quickly tweak the code to create problems for us!

The tool is written in C++ and uses the Windows Debugging framework to execute the code. It can be used with WinDbg as a ‘plugin’ in order to help automate the analysis process.

If you want to know more about the tool, feel free to contact me or comment below.
## Download 
Download all the DLLs from this repo. 
## Usage
