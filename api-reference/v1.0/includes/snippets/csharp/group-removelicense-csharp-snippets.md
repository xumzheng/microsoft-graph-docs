---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AssignLicensePostRequestBody
{
	AddLicenses = new List<>
	{
	},
	RemoveLicenses = new List<>
	{
		"c7df2760-2c81-4ef7-b578-5b5392b571df",
		"b05e124f-c7cc-45a0-a6aa-8cf78c946968",
	},
};
var result = await graphClient.Groups["group-id"].AssignLicense.PostAsync(requestBody);


```