---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new DriveItem
{
	Name = "Shared legal agreements",
};
var result = await graphClient.Drive.Items["driveItem-id"].PatchAsync(requestBody);


```