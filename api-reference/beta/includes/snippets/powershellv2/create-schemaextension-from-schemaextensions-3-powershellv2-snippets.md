---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.SchemaExtensions

$params = @{
	Id = "courses"
	Description = "Graph Learn training courses extensions"
	TargetTypes = @(
		"Group"
	)
	Owner = "50897f70-a455-4adf-87bc-4cf17091d5ac"
	Properties = @(
		@{
			Name = "courseId"
			Type = "Integer"
		}
		@{
			Name = "courseName"
			Type = "String"
		}
		@{
			Name = "courseType"
			Type = "String"
		}
	)
}

New-MgBetaSchemaExtension -BodyParameter $params

```