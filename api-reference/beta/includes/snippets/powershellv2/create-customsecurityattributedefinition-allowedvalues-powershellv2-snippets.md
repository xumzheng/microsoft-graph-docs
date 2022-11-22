---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.DirectoryManagement

$params = @{
	AttributeSet = "Engineering"
	Description = "Active projects for user"
	IsCollection = $true
	IsSearchable = $true
	Name = "Project"
	Status = "Available"
	Type = "String"
	UsePreDefinedValuesOnly = $true
	AllowedValues = @(
		@{
			Id = "Alpine"
			IsActive = $true
		}
		@{
			Id = "Baker"
			IsActive = $true
		}
		@{
			Id = "Cascade"
			IsActive = $true
		}
	)
}

New-MgBetaDirectoryCustomSecurityAttributeDefinition -BodyParameter $params

```