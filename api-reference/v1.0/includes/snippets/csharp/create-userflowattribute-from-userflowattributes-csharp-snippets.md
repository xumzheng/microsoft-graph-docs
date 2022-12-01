---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new IdentityUserFlowAttribute
{
	DisplayName = "Hobby",
	Description = "Your hobby",
	DataType = IdentityUserFlowAttributeDataType.String,
};
var result = await graphClient.Identity.UserFlowAttributes.PostAsync(requestBody);


```