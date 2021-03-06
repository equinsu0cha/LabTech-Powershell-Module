# Start-LTService
## SYNOPSIS
This function will start the LabTech Services.
## SYNTAX
```powershell
Start-LTService [-WhatIf] [-Confirm] [<CommonParameters>]
```
## DESCRIPTION
This function will verify that the LabTech services are present.
It will then check for any process that is using the LTTray port (Default 42000) and kill it.
Next it will start the services.
## PARAMETERS
### -WhatIf &lt;SwitchParameter&gt;

```
Required                    false
Position                    named
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -Confirm &lt;SwitchParameter&gt;

```
Required                    false
Position                    named
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
## NOTES
Version:        1.5

Author:         Chris Taylor

Website:        labtechconsulting.com

Creation Date:  3/14/2016

Purpose/Change: Initial script development



Update Date: 5/11/2017

Purpose/Change: added check for non standard port number and set services to auto start



Update Date: 6/1/2017

Purpose/Change: Updates for better overall compatibility, including better support for PowerShell V2



Update Date: 12/14/2017

Purpose/Change: Will increment the tray port if a conflict is detected.



Update Date: 2/1/2018

Purpose/Change: Added support for -WhatIf. Added Service Control Command to request agent check-in immediately after startup.



Update Date: 3/21/2018

Purpose/Change: Removed ErrorAction Override 
