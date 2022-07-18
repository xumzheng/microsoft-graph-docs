---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new RetentionEventType
{
	@odata.type = "#microsoft.graph.security.retentionEventType",
	DisplayName = "String",
	Description = "String",
	CreatedBy = new IdentitySet
	{
		@odata.type = "microsoft.graph.identitySet",
	},
};
var result = await graphClient.Security.TriggerTypes.RetentionEventTypes.PostAsync(requestBody);


```