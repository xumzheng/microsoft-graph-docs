---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.Governance

$params = @{
	DisplayName = "All Contoso volunteers - Terms of use"
	IsViewingBeforeAcceptanceRequired = $true
}

Update-MgBetaIdentityGovernanceTermOfUseAgreement -AgreementId $agreementId -BodyParameter $params

```