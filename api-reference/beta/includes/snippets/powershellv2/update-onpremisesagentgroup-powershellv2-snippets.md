---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Applications

$params = @{
	displayName = "Group New Name"
}

Update-MgBetaOnPremisePublishingProfileAgentGroup -OnPremisesPublishingProfileId $onPremisesPublishingProfileId -OnPremisesAgentGroupId $onPremisesAgentGroupId -BodyParameter $params

```