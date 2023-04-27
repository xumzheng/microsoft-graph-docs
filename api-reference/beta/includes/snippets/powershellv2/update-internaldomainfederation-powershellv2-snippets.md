---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.DirectoryManagement

$params = @{
	displayName = "Contoso name change"
	federatedIdpMfaBehavior = "acceptIfMfaDoneByFederatedIdp"
}

Update-MgBetaDomainFederationConfiguration -DomainId $domainId -InternalDomainFederationId $internalDomainFederationId -BodyParameter $params

```