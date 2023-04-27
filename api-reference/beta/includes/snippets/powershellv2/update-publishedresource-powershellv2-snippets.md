---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Applications

$params = @{
	displayName = "Demo provisioning (updated)"
}

Update-MgBetaOnPremisePublishingProfilePublishedResource -OnPremisesPublishingProfileId $onPremisesPublishingProfileId -PublishedResourceId $publishedResourceId -BodyParameter $params

```