---
external help file: Az.DiagnosticSetting.psm1-help.xml
Module Name: Az.Monitor
online version: https://learn.microsoft.com/powershell/module/az.DiagnosticSetting/new-AzDiagnosticSettingMetricSettingsObject
schema: 2.0.0
content_git_url: https://github.com/Azure/azure-powershell/blob/main/src/Monitor/Monitor/help/New-AzDiagnosticSettingMetricSettingsObject.md
original_content_git_url: https://github.com/Azure/azure-powershell/blob/main/src/Monitor/Monitor/help/New-AzDiagnosticSettingMetricSettingsObject.md
---

# New-AzDiagnosticSettingMetricSettingsObject

## SYNOPSIS
Create an in-memory object for MetricSettings.

> [!NOTE]
>This is the previous version of our documentation. Please consult [the most recent version](/powershell/module/az.monitor/new-azdiagnosticsettingmetricsettingsobject) for up-to-date information.

## SYNTAX

```
New-AzDiagnosticSettingMetricSettingsObject -Enabled <Boolean> [-Category <String>]
 [-RetentionPolicyDay <Int32>] [-RetentionPolicyEnabled <Boolean>] [-TimeGrain <TimeSpan>] [<CommonParameters>]
```

## DESCRIPTION
Create an in-memory object for MetricSettings.

## EXAMPLES

### Example 1: Create metric setting object
```powershell
New-AzDiagnosticSettingMetricSettingsObject -Enabled $true -Category AllMetrics -RetentionPolicyDay 7 -RetentionPolicyEnabled $true
```

Create metric setting object, to get supported categories for resource, please see `Get-AzDiagnosticSettingCategory`

## PARAMETERS

### -Category
Name of a Diagnostic Metric category for a resource type this setting is applied to.
To obtain the list of Diagnostic metric categories for a resource, first perform a GET diagnostic settings operation.

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
a value indicating whether this category is enabled.

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

### -RetentionPolicyDay
the number of days for the retention in days.
A value of 0 will retain the events indefinitely.

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RetentionPolicyEnabled
a value indicating whether the retention policy is enabled.

```yaml
Type: System.Boolean
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TimeGrain
the timegrain of the metric in ISO8601 format.

```yaml
Type: System.TimeSpan
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### Microsoft.Azure.PowerShell.Cmdlets.Monitor.DiagnosticSetting.Models.Api20210501Preview.MetricSettings

## NOTES

ALIASES

## RELATED LINKS
