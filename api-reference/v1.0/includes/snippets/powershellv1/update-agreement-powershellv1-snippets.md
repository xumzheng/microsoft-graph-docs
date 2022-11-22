---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
	DisplayName = "All Contoso volunteers - Terms of use"
	IsViewingBeforeAcceptanceRequired = $true
}

Update-MgIdentityGovernanceTermOfUseAgreement -AgreementId $agreementId -BodyParameter $params

```