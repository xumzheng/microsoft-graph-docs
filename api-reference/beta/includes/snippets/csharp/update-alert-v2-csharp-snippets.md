---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Models.Security.Alert
{
	AssignedTo = "secAdmin@contoso.onmicrosoft.com",
	Classification = Microsoft.Graph.Beta.Models.Security.AlertClassification.TruePositive,
	Determination = Microsoft.Graph.Beta.Models.Security.AlertDetermination.Malware,
	Status = Microsoft.Graph.Beta.Models.Security.AlertStatus.InProgress,
};
await graphClient.Security.Alerts_v2["alert-id"].PatchAsync(requestBody);


```