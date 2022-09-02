---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AllowedValue
{
	IsActive = false,
};
await graphClient.DirectoryObject.CustomSecurityAttributeDefinitions["customSecurityAttributeDefinition-id"].AllowedValues["allowedValue-id"].PatchAsync(requestBody);


```