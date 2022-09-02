---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new IdentityUserFlowAttributeAssignment
{
	UserInputType = IdentityUserFlowAttributeInputType.Textbox,
};
await graphClient.Identity.B2xUserFlows["b2xIdentityUserFlow-id"].UserAttributeAssignments["identityUserFlowAttributeAssignment-id"].PatchAsync(requestBody);


```