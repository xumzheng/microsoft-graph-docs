---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Users

$params = @{
	xboxGamerTag = "FierceAdele"
	linkedInProfile = "www.linkedin.com/in/testlinkedinprofile"
}

Update-MgUserExtension -UserId $userId -ExtensionId $extensionId -BodyParameter $params

```