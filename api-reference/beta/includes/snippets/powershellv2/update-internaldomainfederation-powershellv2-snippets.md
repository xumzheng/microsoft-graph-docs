---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.DirectoryManagement

$params = @{
	DisplayName = "Contoso name change"
	FederatedIdpMfaBehavior = "acceptIfMfaDoneByFederatedIdp"
}

Update-MgBetaDomainFederationConfiguration -DomainId $domainId -InternalDomainFederationId $internalDomainFederationId -BodyParameter $params

```