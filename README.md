# RCT (Right Click Tools) for Updates + Software Update Extension

## English help

## How it looks

- Updates required for members:

![Updates required for members](screenshots/rct-01.png?raw=true "Updates required for the computer")

![Updates required for device](screenshots/SuExt+rct-01.png?raw=true "Updates required for the device")

![Updates required for device collection](screenshots/SuExt+rct-02.png?raw=true "Updates required for the device collection")

- Update compliance status:

![Update compliance status](screenshots/rct-03.png?raw=true "Update compliance status")

![Update compliance status: Required](screenshots/SuExt+rct-03.png?raw=true "Update compliance status")

![Update compliance status: Required](screenshots/SuExt+rct-04.png?raw=true "Update compliance status")

- Create SUG for Collection:

![Create SUG for Collection](screenshots/rct-04.png?raw=true "Create SUG for Collection")

... and more samples from ScreenShots folder

## How to install

- Backup the Console folder "C:\Program Files (x86)\Microsoft Configuration Manager\AdminConsole" or "C:\Program Files (x86)\Microsoft Endpoint Manager\AdminConsole"
- Download ZIP-file. Press "Clone or Download" button / "Download ZIP".
- **Unblock downloaded file** from Properties / Unblock
- Extract All
- For the RCT tool, right-click on "install.bat" and select "Run as Administrator". The bat file will copy RCT *.ps1 and *.xml files.
- For the Console extension, right-click on "install-SuExtension.bat" and select "Run as Administrator". The bat file will copy Software Update Console extension xml-files and ps1 for RCT. Only if your Console supported ("Xml-SuExtension" - the subfolder with Supported version. Now is 1906+ )
- Restart the CM-Console

Happy updates!

## Modified Console Objects

Nodes:

- \Assets and Compliance\Overview\Devices\<Selected Device>\<Tab: "Updates: Required">
- \Assets and Compliance\Overview\Device Collections\<Selected Collection>\<Tab: "Updates: Required">
- \Software Library\Overview\Software Updates\All Software Updates\<Selected Update>\<Tab: "Compliance: Required">
- \Software Library\Overview\Software Updates\Software Update Groups\<Selected SUG>\<Tab: "Compliance: Required">

Navigation Aliases:

- MembersOfCollection: \Assets and Compliance\Overview\Devices\<Opened Collection>\<Selected Device>\<Tab: "Updates: Required">
- OpenSoftwareUpdatePackage: \Software Library\Overview\Software Updates\All Software Updates\<Opened SUP>\<Selected Update>\<Tab: "Compliance: Required">
- OpenUpdateGroup: \Software Library\Overview\Software Updates\All Software Updates\<Opened SUG>\<Selected Update>\<Tab: "Compliance: Required">

Additions:

- OpenUpdateGroup: \Software Library\Overview\Software Updates\All Software Updates\<Opened SUG>\<Selected Update>\<RMC: "Publish Third-Party Software Update Content">

Where:

- SUG - Software Update Group
- SUP - Software Update Package
- Tab - TabPage
- RMC - Right Mouse Click

## Russian

## RCT (Right Click Tools) для работы с обновлениями

https://skorotkov.wordpress.com/2018/07/11/sccm-sug-rct-required-updates-and-update-status/

https://skorotkov.wordpress.com/2018/08/12/sccm-sug-rct-updates-and-compliance-part2/

https://skorotkov.wordpress.com/2020/01/20/sccm-sug-rct-suext-updates-and-compliance-part3/

Happy updates!
