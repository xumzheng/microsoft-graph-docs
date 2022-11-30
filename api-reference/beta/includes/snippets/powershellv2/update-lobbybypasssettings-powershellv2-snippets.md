---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.CloudCommunications

$params = @{
	LobbyBypassSettings = @{
		IsDialInBypassEnabled = $true
	}
}

# A UPN can also be used as -UserId.
Update-MgBetaUserOnlineMeeting -UserId $userId -OnlineMeetingId $onlineMeetingId -BodyParameter $params

```