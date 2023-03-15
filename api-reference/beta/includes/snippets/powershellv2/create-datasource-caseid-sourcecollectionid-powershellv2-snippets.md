---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Compliance

$params = @{
	"@odata.type" = "microsoft.graph.ediscovery.userSource"
	Email = "badguy@contoso.com"
}

New-MgBetaComplianceEdiscoveryCaseSourceCollectionAdditionalSource -CaseId $caseId -SourceCollectionId $sourceCollectionId -BodyParameter $params

```