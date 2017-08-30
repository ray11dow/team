﻿# Set-ReleaseStatus

## SYNOPSIS
Sets the status of a release to Active or Abandoned.

## SYNTAX

### Parameter Set 1
```
Set-ReleaseStatus [-ProjectName] <String> [-Id] <Int32[]> [[-Status] <String>] [-Force]
```

## DESCRIPTION
Set-ReleaseStatus lets you set the status of the release to Acitve or Abandoned.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
PS C:\\\>
```powershell
Set-ReleaseStatus -Id 5 -status Abandoned
```

This command will set the status of release with id 5 to Abandoned.

## PARAMETERS

### Id
Specifies one or more releases by ID. To specify multiple IDs, 
use commas to separate the IDs. To find the ID of a release
type Get-Release.

```yaml
Type: Int32[]
Parameter Sets: Parameter Set 1
Aliases: 

Required: true
Position: 0
Default Value: 
Pipeline Input: True (ByPropertyName)
```

### Status
The status to set for the release Active or Abandoned.

```yaml
Type: String
Parameter Sets: Parameter Set 1
Aliases: 

Required: false
Position: 1
Default Value: 
Pipeline Input: false
```

### Force
Removes the specified build without prompting for confirmation.
By default, Set-ReleaseStatus prompts for confirmation before 
changing the status.

```yaml
Type: SwitchParameter
Parameter Sets: Parameter Set 1
Aliases: 

Required: false
Position: named
Default Value: 
Pipeline Input: false
```

### ProjectName
Specifies the team project for which this function operates.

You can tab complete from a list of available projects.

You can use Set-DefaultProject to set a default project so
you do not have to pass the ProjectName with each call.

```yaml
Type: String
Parameter Sets: Parameter Set 1
Aliases: 

Required: true
Position: 0
Default Value: 
Pipeline Input: True (ByPropertyName)
Dynamic: true
```

## INPUTS

### System.Int32[]
System.String


## OUTPUTS

### System.Object


## NOTES

## RELATED LINKS


*Generated by: PowerShell HelpWriter 2017 v2.1.36*