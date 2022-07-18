---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Alert
{
	AssignedTo = "String",
	ClosedDateTime = DateTimeOffset.Parse("String (timestamp)"),
	Comments = new List<String>
	{
		"String",
	}
	Feedback = "@odata.type: microsoft.graph.alertFeedback",
	Status = "@odata.type: microsoft.graph.alertStatus",
	Tags = new List<String>
	{
		"String",
	}
	VendorInformation = new SecurityVendorInformation
	{
		Provider = "String",
		Vendor = "String",
	},
};
await graphClient.Security.Alerts["alert-id"].PatchAsync(requestBody);


```