---
external help file: KaceSMA-help.xml
Module Name: KaceSMA
online version: https://github.com/ArtisanByteCrafter/KaceSMA/blob/master/docs/Set-SmaAsset.md
schema: 2.0.0
---

# Set-SmaAsset

## SYNOPSIS

## SYNTAX

```
Set-SmaAsset -Id <Int32> [-Body] <Hashtable> [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
Updates an SMA asset.

## EXAMPLES

### EXAMPLE 1
```powershell
PS> $SetAssetBody = @{
    'Assets' = @(
        @{
        'id'          = 10000
        'field_10000' = 'My String'
        }
    )
}

PS> Set-SmaAsset -Body $SetAssetBody
```

Updates the field 'field_10000' with string 'My String' on asset with ID 1234. Get asset field identities using Get-SmaAsset with query parameters `"?shaping=asset all"` on a similar asset if needed.

## PARAMETERS

### -Body
A hashtable-formatted payload containing the asset information.
See example.

```yaml
Type: Hashtable
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Id
Specifies the id of the item to query.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: AssetId

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### PSCustomObject
## NOTES

## RELATED LINKS
