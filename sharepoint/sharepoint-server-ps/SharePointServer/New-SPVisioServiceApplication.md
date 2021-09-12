---
external help file: Microsoft.Office.Visio.Server.dll-help.xml
module name: SharePointServer
online version: https://docs.microsoft.com/powershell/module/sharepoint-server/new-spvisioserviceapplication
applicable: SharePoint Server Subscription Edition
title: New-SPVisioServiceApplication
schema: 2.0.0
---

# New-SPVisioServiceApplication

## SYNOPSIS
Adds a new Visio Services application to a farm.


## SYNTAX

```
New-SPVisioServiceApplication -ApplicationPool <SPIisWebServiceApplicationPoolPipeBind> [-AddToDefaultGroup]
 [-AssignmentCollection <SPAssignmentCollection>] [-Confirm] [-Name <String>] [-WhatIf] [<CommonParameters>]
```

## DESCRIPTION
The `New-SPVisioServiceApplication` cmdlet adds a new Visio Services application to a farm.

For permissions and the most current information about Windows PowerShell for SharePoint Products, see the online documentation at [SharePoint Server Cmdlets](https://docs.microsoft.com/powershell/sharepoint/sharepoint-server/sharepoint-server-cmdlets).


## EXAMPLES

### ----------------EXAMPLE 1---------------------
```powershell
New-SPVisioServiceApplication -Identity 'Visio Graphics Service Application' -ApplicationPool 'SharePoint Web Services Default' -CreateDefaultProxy
```

This example creates a new Visio Services application named 'Visio Graphics Service Application' and also creates a service application proxy associated with it.


## PARAMETERS

### -ApplicationPool
Specifies the existing IIS application pool in which to run the Web service for the service application.

The type must be a valid GUID, in the form 12345678-90ab-cdef-1234-567890bcdefgh; a valid name of an application pool (for example, AppPoolName1); or an instance of a valid IISWebServiceApplicationPool object.

```yaml
Type: SPIisWebServiceApplicationPoolPipeBind
Parameter Sets: (All)
Aliases: 
Applicable: SharePoint Server Subscription Edition

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -AddToDefaultGroup
Specifies that a default proxy is created for the new Visio Services application.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 
Applicable: SharePoint Server Subscription Edition

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -AssignmentCollection
Manages objects for the purpose of proper disposal.
Use of objects, such as SPWeb or SPSite, can use large amounts of memory and use of these objects in Windows PowerShell scripts requires proper memory management.
Using the SPAssignment object, you can assign objects to a variable and dispose of the objects after they are needed to free up memory.
When SPWeb, SPSite, or SPSiteAdministration objects are used, the objects are automatically disposed of if an assignment collection or the Global parameter is not used.

When the Global parameter is used, all objects are contained in the global store.
If objects are not immediately used, or disposed of by using the `Stop-SPAssignment` command, an out-of-memory scenario can occur.

```yaml
Type: SPAssignmentCollection
Parameter Sets: (All)
Aliases: 
Applicable: SharePoint Server Subscription Edition

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before executing the command.
For more information, type the following command: `get-help about_commonparameters`

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf
Applicable: SharePoint Server Subscription Edition

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
Specifies the Visio Services application to create.

The type must be a valid name of a Visio Service application; for example, MyVisioService1.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 
Applicable: SharePoint Server Subscription Edition

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -WhatIf
Displays a message that describes the effect of the command instead of executing the command.
For more information, type the following command: `get-help about_commonparameters`

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi
Applicable: SharePoint Server Subscription Edition

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (https://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS