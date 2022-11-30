---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.Governance

$params = @{
	DisplayName = "Contoso ToU for guest users"
	IsViewingBeforeAcceptanceRequired = $true
	Files = @(
		@{
			FileName = "TOU.pdf"
			Language = "en"
			IsDefault = $true
			FileData = @{
				Data = [System.Text.Encoding]::ASCII.GetBytes("SGVsbG8gd29ybGQ=//truncated-binary")
			}
		}
	)
}

New-MgBetaIdentityGovernanceTermOfUseAgreement -BodyParameter $params

```