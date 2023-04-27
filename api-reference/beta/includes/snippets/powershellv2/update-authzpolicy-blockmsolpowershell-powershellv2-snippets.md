---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.SignIns

$params = @{
	blockMsolPowerShell = $true
}

Update-MgBetaPolicyAuthorizationPolicy -AuthorizationPolicyId $authorizationPolicyId -BodyParameter $params

```