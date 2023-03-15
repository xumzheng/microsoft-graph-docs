---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.CloudCommunications

$params = @{
	"@odata.type" = "#microsoft.graph.call"
	CallbackUri = "https://bot.contoso.com/callback"
	RequestedModalities = @(
		"audio"
	)
	MediaConfig = @{
		"@odata.type" = "#microsoft.graph.serviceHostedMediaConfig"
		PreFetchMedia = @(
		)
	}
	MeetingInfo = @{
		"@odata.type" = "#microsoft.graph.joinMeetingIdMeetingInfo"
		JoinMeetingId = "1234567"
		Passcode = $null
	}
	TenantId = "86dc81db-c112-4228-9222-63f3esaa1edb"
}

New-MgBetaCommunicationCall -BodyParameter $params

```