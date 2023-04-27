---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	displayName = "UpdateClaimsPolicy"
}

Update-MgPolicyClaimMappingPolicy -ClaimsMappingPolicyId $claimsMappingPolicyId -BodyParameter $params

```