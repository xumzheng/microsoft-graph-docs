---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new IdentityUserFlowAttributeAssignment
{
	IsOptional = false,
	RequiresVerification = false,
	UserInputType = IdentityUserFlowAttributeInputType.Textbox,
	DisplayName = "Shoe size",
	UserAttributeValues = new List<>
	{
	},
	UserAttribute = new UserAttribute
	{
		Id = "extension_guid_shoeSize",
	},
};
var result = await graphClient.Identity.B2xUserFlows["b2xIdentityUserFlow-id"].UserAttributeAssignments.PostAsync(requestBody);


```