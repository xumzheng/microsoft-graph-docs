---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.ChangeNotifications

$params = @{
	ExpirationDateTime = [System.DateTime]::Parse("2016-11-22T18:23:45.9356913Z")
}

Update-MgBetaSubscription -SubscriptionId $subscriptionId -BodyParameter $params

```