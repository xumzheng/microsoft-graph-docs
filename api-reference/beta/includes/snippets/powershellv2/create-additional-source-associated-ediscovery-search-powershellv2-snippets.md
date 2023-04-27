---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Security

$params = @{
	"@odata.type" = "microsoft.graph.security.siteSource"
}

New-MgBetaSecurityCaseEdiscoveryCaseSearchAdditionalSource -EdiscoveryCaseId $ediscoveryCaseId -EdiscoverySearchId $ediscoverySearchId -BodyParameter $params

```