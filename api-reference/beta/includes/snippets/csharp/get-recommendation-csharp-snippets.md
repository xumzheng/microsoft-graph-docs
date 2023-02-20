---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var recommendations = await graphClient.Directory.Recommendations
	.Request()
	.Filter("id eq '0cb31920-84b9-471f-a6fb-468c1a847088_Microsoft.Identity.IAM.Insights.TurnOffPerUserMFA'")
	.Expand("impactedResources")
	.GetAsync();

```