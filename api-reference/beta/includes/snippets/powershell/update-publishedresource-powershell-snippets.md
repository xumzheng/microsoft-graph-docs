---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
	displayName = "Demo provisioning (updated)"
}

Update-MgOnPremisePublishingProfilePublishedResource -OnPremisesPublishingProfileId $onPremisesPublishingProfileId -PublishedResourceId $publishedResourceId -BodyParameter $params

```