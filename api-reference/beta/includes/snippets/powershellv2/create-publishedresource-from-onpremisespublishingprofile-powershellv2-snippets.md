---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Applications

$params = @{
	displayName = "New provisioning"
	resourceName = "domain1.contoso.com"
}

New-MgBetaOnPremisePublishingProfilePublishedResource -OnPremisesPublishingProfileId $onPremisesPublishingProfileId -BodyParameter $params

```