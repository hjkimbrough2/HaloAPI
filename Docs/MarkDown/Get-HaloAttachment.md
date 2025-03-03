---
external help file: HaloAPI-help.xml
Module Name: HaloAPI
online version:
schema: 2.0.0
---

# Get-HaloAttachment

## SYNOPSIS
Gets attachments from the Halo API.

## SYNTAX

### Multi (Default)
```
Get-HaloAttachment -TicketID <Int64> [-ActionID <Int64>] [-Type <Int64>] [-UniqueID <Int64>]
 [<CommonParameters>]
```

### SinglePath
```
Get-HaloAttachment -AttachmentID <Int64> -OutPath <String> [<CommonParameters>]
```

### SingleFile
```
Get-HaloAttachment -AttachmentID <Int64> -OutFile <String> [<CommonParameters>]
```

### Single
```
Get-HaloAttachment -AttachmentID <Int64> [-IncludeDetails] [<CommonParameters>]
```

## DESCRIPTION
Retrieves attachments from the Halo API - supports a variety of filtering parameters.

## EXAMPLES

### Example 1
```powershell
PS C:\> {{ Add example code here }}
```

{{ Add example description here }}

## PARAMETERS

### -ActionID
Returns attachments from the action ID specified (requires ticket_id)

```yaml
Type: Int64
Parameter Sets: Multi
Aliases: action_id

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -AttachmentID
Attachment ID

```yaml
Type: Int64
Parameter Sets: SinglePath, SingleFile, Single
Aliases:

Required: True
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -IncludeDetails
Include extra objects in the result.

```yaml
Type: SwitchParameter
Parameter Sets: Single
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -OutFile
Allow Writing Directly to File, using the specified path and file name eg c:\temp\myfile.txt

```yaml
Type: String
Parameter Sets: SingleFile
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -OutPath
Allow Writing Directly to File, using the specified path and the original file name eg c:\temp\

```yaml
Type: String
Parameter Sets: SinglePath
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TicketID
Returns attachments from the ticket ID specified

```yaml
Type: Int64
Parameter Sets: Multi
Aliases: ticket_id

Required: True
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -Type
Returns attachments of the specified type

```yaml
Type: Int64
Parameter Sets: Multi
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -UniqueID
Returns an attachment with the unique ID specified

```yaml
Type: Int64
Parameter Sets: Multi
Aliases: unique_id

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### A powershell object containing the response.
## NOTES

## RELATED LINKS
