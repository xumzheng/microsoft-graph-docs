---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.SignIns

$params = @{
	"@odata.type" = "#microsoft.graph.mobilityManagementPolicy"
	ComplianceUrl = "https://portal.mg.contoso.com/?portalAction=Compliance"
	DiscoveryUrl = "https://enrollment.mg.contoso.com/enrollmentserver/discovery.svc"
	TermsOfUseUrl = "https://portal.mg.contoso.com/TermsofUse.aspx"
}

Update-MgBetaPolicyMobileAppManagementPolicy -MobilityManagementPolicyId $mobilityManagementPolicyId -BodyParameter $params

```