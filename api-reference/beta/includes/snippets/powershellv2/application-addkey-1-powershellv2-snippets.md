---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Applications

$params = @{
	KeyCredential = @{
		Type = "AsymmetricX509Cert"
		Usage = "Verify"
		Key = [System.Text.Encoding]::ASCII.GetBytes("MIIDYDCCAki...")
	}
	PasswordCredential = $null
	Proof = "eyJ0eXAiOiJ..."
}

Add-MgBetaApplicationKey -ApplicationId $applicationId -BodyParameter $params

```