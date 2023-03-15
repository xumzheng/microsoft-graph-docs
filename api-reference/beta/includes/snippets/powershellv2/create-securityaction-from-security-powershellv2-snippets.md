---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Security

$params = @{
	Name = "BlockIp"
	ActionReason = "Test"
	Parameters = @(
		@{
			Name = "IP"
			Value = "1.2.3.4"
		}
	)
	VendorInformation = @{
		Provider = "Windows Defender ATP"
		Vendor = "Microsoft"
	}
}

New-MgBetaSecurityAction -BodyParameter $params

```