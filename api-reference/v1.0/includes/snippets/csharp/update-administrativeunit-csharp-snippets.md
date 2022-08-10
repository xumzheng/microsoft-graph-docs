---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AdministrativeUnit
{
	DisplayName = "Greater Seattle District Technical Schools",
};
await graphClient.Directory.AdministrativeUnits["administrativeUnit-id"].PatchAsync(requestBody);


```