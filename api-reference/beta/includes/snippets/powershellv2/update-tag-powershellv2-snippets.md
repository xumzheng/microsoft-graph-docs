---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Compliance

$params = @{
	Description = "This is an updated description."
}

Update-MgBetaComplianceEdiscoveryCaseTag -CaseId $caseId -TagId $tagId -BodyParameter $params

```