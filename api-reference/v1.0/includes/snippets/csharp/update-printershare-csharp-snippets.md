---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new PrinterShare
{
	DisplayName = "PrinterShare Name",
	AllowAllUsers = false,
	AdditionalData = new Dictionary<string, object>
	{
		{
			"printer@odata.bind" , "https://graph.microsoft.com/v1.0/print/printers/{printerId}"
		},
	},
};
await graphClient.Print.Shares["printerShare-id"].PatchAsync(requestBody);


```