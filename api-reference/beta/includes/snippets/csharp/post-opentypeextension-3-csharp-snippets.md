---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Extension
{
	@odata.type = "microsoft.graph.openTypeExtension",
	AdditionalData = new()
	{
		{"extensionName", "Com.Contoso.Deal"},
		{"companyName", "Alpine Skis"},
		{"dealValue", },
		{"expirationDate", "2015-07-03T13:04:00.000Z"},
	}
};
var result = await graphClient.Groups["group-id"].Events["event-id"].Extensions.PostAsync(requestBody);


```