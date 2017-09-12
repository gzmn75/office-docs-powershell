---
external help file: sharepoint.xml
online version: 
schema: 2.0.0
---

# Set-SPServiceApplicationPool

## SYNOPSIS
Below Content Applies To: SharePoint Server 2013

## SYNTAX

```
Set-SPServiceApplicationPool [-Identity] <SPIisWebServiceApplicationPoolPipeBind>
 [[-Account] <SPProcessAccountPipeBind>] [-AssignmentCollection <SPAssignmentCollection>] [-Confirm] [-WhatIf]
```

## DESCRIPTION
The Set-SPServiceApplicationPool cmdlet changes the account used for the Identity of the specified application pool.

For permissions and the most current information about Windows PowerShell for SharePoint Products, see the online documentation at http://go.microsoft.com/fwlink/p/?LinkId=251831 (http://go.microsoft.com/fwlink/p/?LinkId=251831).

## EXAMPLES

### ------------------EXAMPLE----------------------- (SharePoint Server 2013)
```
C:\PS>Set-SPServiceApplicationPool  TestServiceWebApplicationPool -Account testdomain\testuser1
```

This example changes the identity of the selected service application pool.

For the Account parameter, the name of a managed account in the farm can be given.
Use the Get-SPManagedAccount cmdlet to view the existing managed account in the farm.
Also, a process account from the output of the Get-SPProcessAccount cmdlet can be used.

### ------------------EXAMPLE----------------------- (SharePoint Server 2016)
```
C:\PS>Set-SPServiceApplicationPool  TestServiceWebApplicationPool -Account testdomain\testuser1
```

This example changes the identity of the selected service application pool.

For the Account parameter, the name of a managed account in the farm can be given.
Use the Get-SPManagedAccount cmdlet to view the existing managed account in the farm.
Also, a process account from the output of the Get-SPProcessAccount cmdlet can be used.

## PARAMETERS

### -Identity
Specifies the identity of the Web service application pool to configure.

```yaml
Type: SPIisWebServiceApplicationPoolPipeBind
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Account
Specifies the credentials that will be the new Identity of the application pool.

```yaml
Type: SPProcessAccountPipeBind
Parameter Sets: (All)
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AssignmentCollection
Manages objects for the purpose of proper disposal.
Use of objects, such as SPWeb or SPSite, can use large amounts of memory and use of these objects in Windows PowerShell scripts requires proper memory management.
Using the SPAssignment object, you can assign objects to a variable and dispose of the objects after they are needed to free up memory.
When SPWeb, SPSite, or SPSiteAdministration objects are used, the objects are automatically disposed of if an assignment collection or the Global parameter is not used.

When the Global parameter is used, all objects are contained in the global store.
If objects are not immediately used, or disposed of by using the Stop-SPAssignment command, an out-of-memory scenario can occur.

```yaml
Type: SPAssignmentCollection
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before executing the command.
For more information, type the following command: get-help about_commonparameters

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Displays a message that describes the effect of the command instead of executing the command.
For more information, type the following command: get-help about_commonparameters

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS
