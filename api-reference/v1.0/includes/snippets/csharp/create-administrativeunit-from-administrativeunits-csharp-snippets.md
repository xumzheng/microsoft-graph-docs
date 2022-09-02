---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AdministrativeUnit
{
	DisplayName = "Seattle District Technical Schools",
	Description = "Seattle district technical schools administration",
	Visibility = "HiddenMembership",
};
var result = await graphClient.DirectoryObject.AdministrativeUnits.PostAsync(requestBody);


```