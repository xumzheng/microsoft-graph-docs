---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Applications

$params = @{
	KeyCredential = @{
		Type = "X509CertAndPassword"
		Usage = "Sign"
		Key = [System.Text.Encoding]::ASCII.GetBytes("MIIDYDCCAki...")
	}
	PasswordCredential = @{
		SecretText = "MKTr0w1..."
	}
	Proof = "eyJ0eXAiOiJ..."
}

Add-MgBetaApplicationKey -ApplicationId $applicationId -BodyParameter $params

```