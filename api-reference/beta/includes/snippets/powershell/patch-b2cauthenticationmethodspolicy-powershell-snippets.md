---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	isEmailPasswordAuthenticationEnabled = $false
	isUserNameAuthenticationEnabled = $true
	isPhoneOneTimePasswordAuthenticationEnabled = $true
}

Update-MgPolicyB2CAuthenticationMethodPolicy -BodyParameter $params

```