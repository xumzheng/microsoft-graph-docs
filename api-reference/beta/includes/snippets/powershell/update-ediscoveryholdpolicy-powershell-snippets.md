---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Security

$params = @{
	description = "updated description"
}

Update-MgSecurityCaseEdiscoveryCaseLegalHold -EdiscoveryCaseId $ediscoveryCaseId -EdiscoveryHoldPolicyId $ediscoveryHoldPolicyId -BodyParameter $params

```