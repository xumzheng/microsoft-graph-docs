---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var result = await graphClient.Directory.CustomSecurityAttributeDefinitions.GetAsync((requestConfiguration) =>
{
	requestConfiguration.QueryParameters.Filter = "attributeSet eq 'Engineering' and status eq 'Available' and type eq 'String'";
});


```