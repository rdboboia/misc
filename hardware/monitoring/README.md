# Monitoring
My custom overlay config for MSI Afterburner + RTSS overlay. Here's a screenshot of how it currently looks (note that it's stil WIP):
![REPO_2025_03_18_08_36_08_894](https://github.com/user-attachments/assets/ccd086a3-6509-4dbf-ab16-71baeaff56b3)

## Software

### MSI Afterburner (v4.6.6 Beta 5)
Note that some APP config is also included.
Here's how the overlay look with MIS Afterburner ONLY:
![REPO_2025_03_18_08_35_52_267](https://github.com/user-attachments/assets/7a984eee-afc3-4d27-8f3a-f731e1485eab)

### RTSS (v7.3.7 Beta 5)
Only custom overlay is included. It must be imported manually from RTSS > Setup > Plugins > OverlayEditor.dll > Setup > Layots > Load.
Some additional configuration might be needed if your data sources don't match mine.

Technically is possible to migrate the entire overlay (MSI AF + RTSS) to RTSS only, but that is A LOT of extra work that I can't invest into right now. However I am currently trying to migrate the graphs to RTSS since this way I can make the graph colors dynamic like the ones that are currently present for GPU temp, GPU HotSopt temp, GPU memory temp.
