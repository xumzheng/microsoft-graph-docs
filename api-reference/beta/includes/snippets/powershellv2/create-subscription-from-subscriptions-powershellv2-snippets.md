---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.ChangeNotifications

$params = @{
	ChangeType = "created"
	NotificationUrl = "https://webhook.azurewebsites.net/api/send/myNotifyClient"
	Resource = "me/mailFolders('Inbox')/messages"
	ExpirationDateTime = [System.DateTime]::Parse("2016-11-20T18:23:45.9356913Z")
	ClientState = "secretClientValue"
	LatestSupportedTlsVersion = "v1_2"
}

New-MgBetaSubscription -BodyParameter $params

```