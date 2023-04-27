---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
	disableUserAccounts = $true
}

Invoke-MgForceDomainDelete -DomainId $domainId -BodyParameter $params

```