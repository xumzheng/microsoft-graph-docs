---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
	DisplayName = "Contoso name change"
	FederatedIdpMfaBehavior = "acceptIfMfaDoneByFederatedIdp"
}

Update-MgDomainFederationConfiguration -DomainId $domainId -InternalDomainFederationId $internalDomainFederationId -BodyParameter $params

```