Updated: 04.2025  
Script created by Salvador Camacho

Update parameter Host with the IP of your Nimbus Windows Virtual Machine or VM that has SiteScope

This script was created with best practices, so it is more resilient, such as:
* Transaction naming
* No third party
* One validation per transaction
* Think times at the end of each transaction to better simulate user behavior
* Nimbus Windows Host IP parametrized

This script uses RDP to connect to the Nimbus Windows VM that has SiteScope, it launches it, clicks on the AOS Monitor folder, exits SiteScope and closes RDP connection

Runtime Settings were set to log only on errors and generate snapshot on errors, think times 75% to 150%

This script has 8 transactions:  
SiteScope-RDP-S01-01 Connect  
SiteScope-RDP-S01-02 Log In  
SiteScope-RDP-S01-03 Click ADM Folder  
SiteScope-RDP-S01-04 Start SiteScope Launcher  
SiteScope-RDP-S01-05 Launch SiteScope  
SiteScope-RDP-S01-06 Click on AOS Monitor Folder  
SiteScope-RDP-S01-07 Exit SiteScope  
SiteScope-RDP-S01-08 Close ADM Folder