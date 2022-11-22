---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.ChangeNotifications

$params = @{
	ExpirationDateTime = [System.DateTime]::Parse("2016-11-22T18:23:45.9356913Z")
}

Update-MgSubscription -SubscriptionId $subscriptionId -BodyParameter $params

```