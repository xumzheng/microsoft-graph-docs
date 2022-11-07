---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Program
{
	DisplayName = "testprogram3",
	Description = "test description",
};
var result = await graphClient.Programs.PostAsync(requestBody);


```