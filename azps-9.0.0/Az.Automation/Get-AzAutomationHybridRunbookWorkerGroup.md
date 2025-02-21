---
external help file: Microsoft.Azure.PowerShell.Cmdlets.Automation.dll-Help.xml
Module Name: Az.Automation
online version: 
schema: 2.0.0
content_git_url: https://github.com/Azure/azure-powershell/blob/main/src/Automation/Automation/help/Get-AzAutomationHybridRunbookWorkerGroup.md
original_content_git_url: https://github.com/Azure/azure-powershell/blob/main/src/Automation/Automation/help/Get-AzAutomationHybridRunbookWorkerGroup.md
---

# Get-AzAutomationHybridRunbookWorkerGroup

## SYNOPSIS
Gets a Hybrid Runbook Worker Group.

> [!NOTE]
>This is the previous version of our documentation. Please consult [the most recent version](/powershell/module/az.automation/get-azautomationhybridrunbookworkergroup) for up-to-date information.

## SYNTAX

### ByAll (Default)
```
Get-AzAutomationHybridRunbookWorkerGroup [-ResourceGroupName] <String> [-AutomationAccountName] <String>
 [-DefaultProfile <IAzureContextContainer>] [<CommonParameters>]
```

### ByName
```
Get-AzAutomationHybridRunbookWorkerGroup [-Name] <String> [-ResourceGroupName] <String>
 [-AutomationAccountName] <String> [-DefaultProfile <IAzureContextContainer>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzAutomationHybridRunbookWorkerGroup** cmdlet gets a Hybrid Runbook Worker Group.

## EXAMPLES

### Example 1
```powershell
Get-AzAutomationHybridRunbookWorkerGroup -AutomationAccountName "Contoso17" -Name "RunbookWorkerGroupName" -ResourceGroupName "ResourceGroup01"
```

## PARAMETERS

### -AutomationAccountName
The automation account name.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -DefaultProfile
The credentials, account, tenant, and subscription used for communication with Azure.

```yaml
Type: Microsoft.Azure.Commands.Common.Authentication.Abstractions.Core.IAzureContextContainer
Parameter Sets: (All)
Aliases: AzContext, AzureRmContext, AzureCredential

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
The Hybrid Runbook Worker Group name

```yaml
Type: System.String
Parameter Sets: ByName
Aliases: WorkerGroup, RunbookWorkerGroup

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ResourceGroupName
The resource group name.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.String

## OUTPUTS

### Microsoft.Azure.Management.Automation.Models.HybridRunbookWorkerGroup

## NOTES

## RELATED LINKS
