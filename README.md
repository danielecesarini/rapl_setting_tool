# Intel RAPL setting tool
Intel RAPL setting tool is a simple python script to configure Intel RAPL throught machine specific registries (MSR). It works for Intel processors on the Linux operating system.

Dependencies
============

It requires three dependencies to work:
- Python 2.7
- MSR module
- terminaltables module for python 

Install
----------

1) Enter in the main directory:

	>$ cd rapl_setting_tool
 
2) Make sure that the msr driver is loaded:

	>$ sudo modprobe msr

3) Install terminaltables module for python:

	>$ sudo pip install terminaltables

4) Run the script with root permissions:

	>$ sudo ./rapl-set

	+-----------------------+----------+
	| Conf Parameter        | Socket 0 |
	+-----------------------+----------+
	| PKG1 power limit (W)  | 255.0    |
	| PKG1 time window (ms) | 9.765625 |
	| PKG1 enable limit     | True     |
	| PKG1 clamping limit   | False    |
	| PKG1 lock             | True     |
	| PKG2 power limit (W)  | 255.0    |
	| PKG2 time window (ms) | 0.0      |
	| PKG2 enable limit     | True     |
	| PKG2 clamping limit   | False    |
	| PKG2 lock             | False    |
	| DRAM power limit (W)  | None     |
	| DRAM time window (ms) | None     |
	| DRAM enable limit     | None     |
	| DRAM lock             | None     |
	| PP0 power limit (W)   | 0.0      |
	| PP0 time window (ms)  | 0.0      |
	| PP0 enable limit      | False    |
	| PP0 clamping limit    | False    |
	| PP0 priority_level    | 0        |
	| PP0 lock              | False    |
	| PP1 power limit (W)   | 0.0      |
	| PP1 time window (ms)  | 0.0      |
	| PP1 enable limit      | False    |
	| PP1 clamping limit    | False    |
	| PP1 priority_level    | 16       |
	| PP1 lock              | False    |
	+-----------------------+----------+
	+-------------------------------+---------------+
	| Arch Parameter                | Value         |
	+-------------------------------+---------------+
	| Time units (ms)               | 0.9765625     |
	| Power units (mW)              | 125.0         |
	| Energy units (uJ)             | 15.2587890625 |
	| PKG Thermal Spec Power (W)    | 95.0          |
	| PKG Minimum Power (W)         | 60.0          |
	| PKG Maximum Power (W)         | 0.0           |
	| PKG Maximum Time Window (ms)  | 0.0           |
	| DRAM Thermal Spec Power (W)   | None          |
	| DRAM Minimum Power (W)        | None          |
	| DRAM Maximum Power (W)        | None          |
	| DRAM Maximum Time Window (ms) | None          |
	+-------------------------------+---------------+
	+-------------------------+---------------+
	| Perf counter            | Socket 0      |
	+-------------------------+---------------+
	| PKG energy (J)          | 24853.1287842 |
	| PKG throttled time (s)  | None          |
	| DRAM energy (J)         | None          |
	| DRAM throttled time (s) | None          |
	| PP0 energy (J)          | 27515.2219391 |
	| PP0 throttled time (s)  | None          |
	| PP1 energy (J)          | 0.0           |
	+-------------------------+---------------+
	
	
