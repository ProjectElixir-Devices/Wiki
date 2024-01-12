![Installation Guide For Project Elixir](https://i.imgur.com/3UmK6nS.png "Installation")

### Installation Guide for Project Elixir on GSI Device

### MEDIATEK DEVICES AND CERTAIN EXYNOS MAY NOT BOOT AT THIS TIME

PREREQUISITES:
* Check Project treble compatibility using [Treble Info](https://play.google.com/store/apps/details?id=tk.hack5.treblecheck)
- Must have A/B partitioning or System-As-Root support
- Must fit into ARM64 architecture requirement. (Future builds may include A64 support)
- Must have at least VNDK28 support.

CLEAN FLASH:
- Download GSI system image
- Extract .xz file
- Boot into recovery
- Flash extracted system.img file as 'System'
- Wipe Cache, Dalvik and format Data
- Reboot system

DIRTY FLASH:
- Download GSI system image
- Extract .xz file
- Boot into recovery
- Wipe dalvik, cache
- Flash the system.img file as 'System'
- Reboot To System
