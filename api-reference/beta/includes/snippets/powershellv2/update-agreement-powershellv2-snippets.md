---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.Governance

$params = @{
	displayName = "All Contoso volunteers - Terms of use"
	isViewingBeforeAcceptanceRequired = $true
}

Update-MgBetaIdentityGovernanceTermOfUseAgreement -AgreementId $agreementId -BodyParameter $params

```