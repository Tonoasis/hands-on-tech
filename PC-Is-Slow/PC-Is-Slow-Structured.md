# PC Is Slow – Startup Applications, Disk Usage, and Services #

## Overview
This lab documents troubleshooting steps taken to diagnose and resolve system performance degradation caused by excessive startup processes, high disk usage, and unnecessary background services. 
The objective was to identify resource bottlenecks and restore optimal system performance using structured diagnostic methods.

## Scenarios / Issue
- System performance was noticeably slow during normal use.  
- Applications took a long time to open or respond.  
- High CPU, memory, or disk usage observed in Task Manager.  
- System occasionally froze or lagged.

## Root Causes Considered
- Too many startup programs launching at boot.  
- High disk usage from background processes.  
- Unnecessary or misconfigured Windows services.  
- Insufficient system resources (CPU/RAM constraints).  
- Windows updates or background tasks consuming resources.

## Troubleshooting Steps
1. **Check system resource usage**  
   - Open Task Manager (`Ctrl + Shift + Esc`).  
   - Review CPU, Memory, and Disk usage.  
   - Identify processes consuming excessive resources.  
   - *((See Screenshot1 + Screenshot2 in `screenshots/` folder)*  

2. **Disable unnecessary startup programs**  
   - Task Manager → Startup tab.  
   - Disable non-essential applications from starting automatically.  
   - *(See Screenshot3 in `screenshots/` folder)*  

3. **Analyze disk usage**  
   - Sort processes by Disk usage in Task Manager.  
   - Identify background processes causing sustained disk activity.  

4. **Review and manage Windows services**  
   - Open Run → `services.msc`.  
   - Identify non-critical services set to Automatic.  
   - Set appropriate services to Manual (where safe and applicable).  
   - *(Reference screenshot4 in `screenshots/` folder)*  

5. **Adjust system performance settings**  
   - Run → `sysdm.cpl`.  
   - System Properties → Advanced → Performance Settings.  
   - Select “Adjust for best performance” to reduce visual effects.  
   - *Impact:* reduces animations/transparency, lowers RAM pressure, reduces disk swap usage, frees CPU/memory resources.  
   - No files deleted, no applications removed.  
   - *(Reference screenshot5 in `screenshots/` folder)* 

6. **Restart the system**  
   - Apply changes and reboot.  
   - Monitor system performance after startup.

## Findings
- Multiple startup applications were consuming resources at boot.  
- Background processes contributed to high disk usage.  
- Visual effects and services increased overall resource consumption.

## Resolution
- Disabled unnecessary startup applications.  
- Adjusted service startup types where appropriate.  
- Optimized system performance settings.  
- Restarted system to apply changes.

## Outcome
- System performance improved noticeably.  
- Reduced CPU and disk usage.  
- Faster application launch times.  
- Improved overall responsiveness and stability.
