---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.DirectoryManagement

$params = @{
	attributeSet = "Engineering"
	description = "Target completion date"
	isCollection = $false
	isSearchable = $true
	name = "ProjectDate"
	status = "Available"
	type = "String"
	usePreDefinedValuesOnly = $false
}

New-MgBetaDirectoryCustomSecurityAttributeDefinition -BodyParameter $params

```