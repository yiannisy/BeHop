# BeHop
Codebase for the BeHop WiFi Project at Stanford University (http://stanford.edu/~yiannisy/behop). 

The BeHop WiFi project has two main goals:
- Enable users to personalize their WiFi experience (setting their own SSID and firewalls) over a shared WiFi infrastructure 
- Enable network administrators to better contol a dense WiFi deployment through a centralized and virtualized architecture. 

The BeHop system consists of wireless APs (running OpenWrt, OpenvSwitch and custom BeHop utilities), a centralized controller (based on the POX OpenFlow controller), and other utilities for data collection, processing and visualization. 

## Authors
- Yiannis Yiakoumis
- Manu Bansal

## Papers
- BeHop : A testbed for dense WiFi networks

## Support
This code is avaialable for informational purposes only. It is not expected to run as is, but rather used as a reference for developers who want to build systems with similar properties. 

## Repo structure
This is a parent repo.
Look at the following submodules for more information:

- behop-pox: Fork of POX OpenFlow controller with modules for WiFi virtualization and ovsdb management. 
- behop-misc: Miscellaneous utilities (including utilities to remotely upgrade AP firmware, add kernel state per station through ovsdb)
- behop-openwrt: Fork of OpenWrt for BeHop support (including ath9k support for virtual BSSIDs and WiFi virtualization).
- behop-dashboard: Management frontend for usage statistics and WiFi events.

