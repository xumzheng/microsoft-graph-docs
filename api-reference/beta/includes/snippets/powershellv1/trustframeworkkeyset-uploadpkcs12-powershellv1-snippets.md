---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	Key = "Base64-encoded-pfx-content"
	Password = "password-value"
}

Invoke-MgUploadTrustFrameworkKeySetPkcs12 -TrustFrameworkKeySetId $trustFrameworkKeySetId -BodyParameter $params

```