---
external help file:
Module Name: Az.SpringCloud
online version: https://learn.microsoft.com/powershell/module/az.springcloud/get-azspringcloudbuildservice
schema: 2.0.0
content_git_url: https://github.com/Azure/azure-powershell/blob/main/src/SpringCloud/help/Get-AzSpringCloudBuildService.md
original_content_git_url: https://github.com/Azure/azure-powershell/blob/main/src/SpringCloud/help/Get-AzSpringCloudBuildService.md
---

# Get-AzSpringCloudBuildService

## SYNOPSIS
Get a build service resource.

## SYNTAX

### Get (Default)
```
Get-AzSpringCloudBuildService -ResourceGroupName <String> -ServiceName <String> [-SubscriptionId <String[]>]
 [-DefaultProfile <PSObject>] [<CommonParameters>]
```

### GetViaIdentity
```
Get-AzSpringCloudBuildService -InputObject <ISpringCloudIdentity> [-DefaultProfile <PSObject>]
 [<CommonParameters>]
```

## DESCRIPTION
Get a build service resource.

## EXAMPLES

### Example 1: Get a build service resource of the enterprise spring cloud
```powershell
Get-AzSpringCloudBuildService -ResourceGroupName springcloudrg -ServiceName sspring-portal01
```

```output
Name    ResourceGroupName ProvisioningState KPackVersion ResourceRequestCpu ResourceRequestMemory
----    ----------------- ----------------- ------------ ------------------ ---------------------
default springcloudrg     Succeeded         0.5.2        2                  4Gi
```

Get a build service resource of the enterprise spring cloud.

### Example 2: Get a build service resource of the enterprise spring cloud by id
```powershell
Get-AzSpringCloudBuildService -InputObject "/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/springcloudrg/providers/Microsoft.AppPlatform/Spring/sspring-portal01/buildServices/default"
```

```output
Name    ResourceGroupName ProvisioningState KPackVersion ResourceRequestCpu ResourceRequestMemory
----    ----------------- ----------------- ------------ ------------------ ---------------------
default springcloudrg     Succeeded         0.5.2        2                  4Gi
```

Get a build service resource of the enterprise spring cloud.

## PARAMETERS

### -DefaultProfile
The credentials, account, tenant, and subscription used for communication with Azure.

```yaml
Type: System.Management.Automation.PSObject
Parameter Sets: (All)
Aliases: AzureRMContext, AzureCredential

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: Microsoft.Azure.PowerShell.Cmdlets.SpringCloud.Models.ISpringCloudIdentity
Parameter Sets: GetViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ResourceGroupName
The name of the resource group that contains the resource.
You can obtain this value from the Azure Resource Manager API or the portal.

```yaml
Type: System.String
Parameter Sets: Get
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ServiceName
The name of the Service resource.

```yaml
Type: System.String
Parameter Sets: Get
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SubscriptionId
Gets subscription ID which uniquely identify the Microsoft Azure subscription.
The subscription ID forms part of the URI for every service call.

```yaml
Type: System.String[]
Parameter Sets: Get
Aliases:

Required: False
Position: Named
Default value: (Get-AzContext).Subscription.Id
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Azure.PowerShell.Cmdlets.SpringCloud.Models.ISpringCloudIdentity

## OUTPUTS

### Microsoft.Azure.PowerShell.Cmdlets.SpringCloud.Models.Api20220401.IBuildService

## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


`INPUTOBJECT <ISpringCloudIdentity>`: Identity Parameter
  - `[AgentPoolName <String>]`: The name of the build service agent pool resource.
  - `[AppName <String>]`: The name of the App resource.
  - `[BindingName <String>]`: The name of the Binding resource.
  - `[BuildName <String>]`: The name of the build resource.
  - `[BuildResultName <String>]`: The name of the build result resource.
  - `[BuildServiceName <String>]`: The name of the build service resource.
  - `[BuilderName <String>]`: The name of the builder resource.
  - `[BuildpackBindingName <String>]`: The name of the Buildpack Binding Name
  - `[BuildpackName <String>]`: The name of the buildpack resource.
  - `[CertificateName <String>]`: The name of the certificate resource.
  - `[ConfigurationServiceName <String>]`: The name of Application Configuration Service.
  - `[DeploymentName <String>]`: The name of the Deployment resource.
  - `[DomainName <String>]`: The name of the custom domain resource.
  - `[Id <String>]`: Resource identity path
  - `[Location <String>]`: the region
  - `[ResourceGroupName <String>]`: The name of the resource group that contains the resource. You can obtain this value from the Azure Resource Manager API or the portal.
  - `[ServiceName <String>]`: The name of the Service resource.
  - `[ServiceRegistryName <String>]`: The name of Service Registry.
  - `[StackName <String>]`: The name of the stack resource.
  - `[SubscriptionId <String>]`: Gets subscription ID which uniquely identify the Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.

## RELATED LINKS

