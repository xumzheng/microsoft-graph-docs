---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
	displayName = "All Contoso volunteers - Terms of use"
	isViewingBeforeAcceptanceRequired = $true
}

Update-MgIdentityGovernanceTermOfUseAgreement -AgreementId $agreementId -BodyParameter $params

```