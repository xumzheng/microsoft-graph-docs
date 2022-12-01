---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new CustomSecurityAttributeDefinition
{
	Description = "Target completion date (YYYY/MM/DD)",
};
var result = await graphClient.DirectoryObject.CustomSecurityAttributeDefinitions["customSecurityAttributeDefinition-id"].PatchAsync(requestBody);


```