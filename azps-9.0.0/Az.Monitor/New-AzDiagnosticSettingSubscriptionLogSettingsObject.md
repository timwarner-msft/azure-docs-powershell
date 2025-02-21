---
external help file: Az.DiagnosticSetting.psm1-help.xml
Module Name: Az.Monitor
online version: https://learn.microsoft.com/powershell/module/az.DiagnosticSetting/new-AzDiagnosticSettingSubscriptionLogSettingsObject
schema: 2.0.0
content_git_url: https://github.com/Azure/azure-powershell/blob/main/src/Monitor/Monitor/help/New-AzDiagnosticSettingSubscriptionLogSettingsObject.md
original_content_git_url: https://github.com/Azure/azure-powershell/blob/main/src/Monitor/Monitor/help/New-AzDiagnosticSettingSubscriptionLogSettingsObject.md
---

# New-AzDiagnosticSettingSubscriptionLogSettingsObject

## SYNOPSIS
Create an in-memory object for SubscriptionLogSettings.

> [!NOTE]
>This is the previous version of our documentation. Please consult [the most recent version](/powershell/module/az.monitor/new-azdiagnosticsettingsubscriptionlogsettingsobject) for up-to-date information.

## SYNTAX

```
New-AzDiagnosticSettingSubscriptionLogSettingsObject -Enabled <Boolean> [-Category <String>]
 [-CategoryGroup <String>] [<CommonParameters>]
```

## DESCRIPTION
Create an in-memory object for SubscriptionLogSettings.

## EXAMPLES

### Example 1: Create subscription log setting object
```powershell
New-AzDiagnosticSettingSubscriptionLogSettingsObject -Category Recommendation -Enabled $true
```

Create subscription log setting object, to get supported categories for resource, please see `Get-AzEventCategory`

## PARAMETERS

### -Category
Name of a Subscription Diagnostic Log category for a resource type this setting is applied to.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CategoryGroup
Name of a Subscription Diagnostic Log category group for a resource type this setting is applied to.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Enabled
a value indicating whether this log is enabled.

```yaml
Type: System.Boolean
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### Microsoft.Azure.PowerShell.Cmdlets.Monitor.DiagnosticSetting.Models.Api20210501Preview.SubscriptionLogSettings

## NOTES

ALIASES

## RELATED LINKS
