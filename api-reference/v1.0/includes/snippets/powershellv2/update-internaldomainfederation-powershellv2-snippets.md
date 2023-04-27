---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
	displayName = "Contoso name change"
	federatedIdpMfaBehavior = "acceptIfMfaDoneByFederatedIdp"
}

Update-MgDomainFederationConfiguration -DomainId $domainId -InternalDomainFederationId $internalDomainFederationId -BodyParameter $params

```