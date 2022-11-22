---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.Governance

$params = @{
	DisplayName = "testprogram3 new name"
}

Update-MgBetaProgram -ProgramId $programId -BodyParameter $params

```