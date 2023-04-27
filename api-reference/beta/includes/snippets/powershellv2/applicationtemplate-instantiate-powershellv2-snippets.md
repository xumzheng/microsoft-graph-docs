---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Applications

$params = @{
	displayName = "testProperties"
}

Invoke-MgBetaInstantiateApplicationTemplate -ApplicationTemplateId $applicationTemplateId -BodyParameter $params

```