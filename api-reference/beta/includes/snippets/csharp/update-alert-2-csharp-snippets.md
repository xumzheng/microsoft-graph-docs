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
	Comments = new List<string>
	{
		"String",
	},
	Feedback = AlertFeedback.AlertFeedback,
	Status = AlertStatus.AlertStatus,
	Tags = new List<string>
	{
		"String",
	},
	VendorInformation = new SecurityVendorInformation
	{
		Provider = "String",
		Vendor = "String",
	},
};
await graphClient.Security.Alerts["alert-id"].PatchAsync(requestBody, (requestConfiguration) =>
{
	requestConfiguration.Headers.Add("Prefer", "return=representation");
});


```