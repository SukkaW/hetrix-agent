# HetrixTools Linux Server Monitoring Agent

Documentation available here: https://docs.hetrixtools.com/category/server-monitor/


-= ChangeLog =-

Version 2.2.3:
- Fixed an issue where SMART test was not properly performed on NVMe disks
- Improved DEBUG mode

Version 2.2.2:
- Improved DEBUG mode
- Fixed an issue where agent would kill its own processes too eagerly, causing data sending issues

Version 2.2.1:
- Fixed an issue where, in some cases, the agent would query `mdadm` for devices not using `mdadm`
- Changed `LC_NUMERIC` locale

Version 2.2.0:
- Introducing DEBUG mode
- Minor fixes and tweaks

Version 2.1.0:
- Introducing ZFS pool health monitoring
- Added `CollectEveryXSeconds` to agent config

Version 2.0.12:
- Fixed an issue with the new service monitoring method introduced in version 2.0.11

Version 2.0.11:
- Improved service monitoring
- Fixed an issue where the metrics collection loop wouldn't break properly

Version 2.0.10: 
- Fixed `division by zero` error for servers without swap
- Replace `ifconfig` with `ip` command for IP address extraction (thanks to @Ry3nlNaToR)

Version 2.0.9: 
- Fixed a bug where in some cases RAID would not be detected properly

Version 2.0.8: 
- Added support for Custom Variables: https://docs.hetrixtools.com/server-agent-custom-variables/ 
- Fixed `needs-restarting` for CloudLinux 8 https://github.com/hetrixtools/agent/commit/7e87b191bab90f682d2f55cc0f2650b5f4f7e0c7 (thanks to @JLHC)

Version 2.0.7:  
- Improved CPU temperature reading by adding support for two third-party software `lm-sensors` and `ipmitool`

Version 2.0.6:
- Improved the `servicestatus` function

Version 2.0.5:
- Improved the `servicestatus` function

Version 2.0.4:
- Fixed a bug where data was not properly being formatted in some cases when monitoring running processes

Version 2.0.3:
- Initial v2 release

Pre v2 changelog:  
https://github.com/hetrixtools/agent/tree/1.6.x
