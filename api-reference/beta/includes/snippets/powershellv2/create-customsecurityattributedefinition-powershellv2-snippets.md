---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.DirectoryManagement

$params = @{
	AttributeSet = "Engineering"
	Description = "Target completion date"
	IsCollection = $false
	IsSearchable = $true
	Name = "ProjectDate"
	Status = "Available"
	Type = "String"
	UsePreDefinedValuesOnly = $false
}

New-MgBetaDirectoryCustomSecurityAttributeDefinition -BodyParameter $params

```