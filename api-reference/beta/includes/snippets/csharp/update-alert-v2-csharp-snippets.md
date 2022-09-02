---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Alert
{
	AssignedTo = "secAdmin@contoso.onmicrosoft.com",
	Classification = AlertClassification.Truepositive,
	Determination = AlertDetermination.Malware,
	Status = AlertStatus.Inprogress,
};
await graphClient.Security.Alerts_v2["alert-id"].PatchAsync(requestBody);


```