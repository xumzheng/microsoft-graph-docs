---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.SignIns

$params = @{
	AutomaticUserConsentSettings = @{
		InboundAllowed = $true
		OutboundAllowed = $true
	}
}

Update-MgBetaPolicyCrossTenantAccessPolicyPartner -CrossTenantAccessPolicyConfigurationPartnerTenantId $crossTenantAccessPolicyConfigurationPartnerTenantId -BodyParameter $params

```