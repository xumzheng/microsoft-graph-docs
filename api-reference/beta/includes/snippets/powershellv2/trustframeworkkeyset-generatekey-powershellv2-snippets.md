---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.SignIns

$params = @{
	Use = "sig"
	Kty = "RSA"
	Nbf = 1508969811
	Exp = 1508969811
}

New-MgBetaTrustFrameworkKeySetKey -TrustFrameworkKeySetId $trustFrameworkKeySetId -BodyParameter $params

```