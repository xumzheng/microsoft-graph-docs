---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new EducationClass
{
	Description = "History - World History 1",
	DisplayName = "World History Level 1",
};
var result = await graphClient.Education.Classes["educationClass-id"].PatchAsync(requestBody);


```