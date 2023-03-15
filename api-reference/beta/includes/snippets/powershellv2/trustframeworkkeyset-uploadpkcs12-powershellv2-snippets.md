---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.SignIns

$params = @{
	Key = "Base64-encoded-pfx-content"
	Password = "password-value"
}

Invoke-MgBetaUploadTrustFrameworkKeySetPkcs12 -TrustFrameworkKeySetId $trustFrameworkKeySetId -BodyParameter $params

```