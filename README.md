# RMMProberScripts
A collection of deployable Windows-based command-line scripts designed to output concerning or important hardware or sensor info; eg. HDD SMART, HW Temps, packet drops, etc. Each tool outputs the associated raw troubleshooting values, along with a PASS or FAIL and proper exit codes. Use with RMM or IT Admin software to alert you when a script check fails. Tested with SyncroMPS and Solarwinds MSP RMM dashboards, but should work with any RMM dashboard that allows running remote scripts and checking output / exit codes. These scripts are ready to upload to your RMM dashboard and by default deloy into the C:\IT folder.

**[TempProber](https://github.com/InviseLabs/RMMProberScripts-TempProber):** Uses OpenHardwareMonitor API to collect and display HW temps along with a PASS or FAIL next to each deployed PC.

**[SMARTProber](https://github.com/InviseLabs/RMMProberScripts-SMARTProber):** Displays HDD/SSD SMART data (pwr on hrs, current pending sectors, etc) with PASS or FAIl of SSDs / HDDs next to each deployed PC.

**[DeviceProber](https://github.com/InviseLabs/RMMProberScripts-DeviceProber):** Scans Device Manager information and reports any devices or drivers with a Warning, Failure, or Missing status attached to them. E.g. sisplays "x devices OK, x MISSING drivers" next to deployed PCs.

**[NICProber](https://github.com/InviseLabs/RMMProberScripts-NICProber):** Reports ethernet adapter connection speed status as 1gbps or 100mbps, which can assist you in troubleshooting network performance or watch for clients that attempt to use old cables or obsolete hardware.

**[ConnectivityProber](https://github.com/InviseLabs/RMMProberScripts-ConnectivityProber):** (Name might change.) Pings Google, or another server of your choice for 50 packets. Reports latency issues, average ms, jitter, and dropped packets. Displays status info next to each deployed PC.

**[FanProber](https://github.com/InviseLabs/RMMProberScripts-FanProber):** ***(COMING SOON)*** Pulls fan speed info, attempts to detect operational issue of the fans, such as intermittent stopping, problematic RPM.
