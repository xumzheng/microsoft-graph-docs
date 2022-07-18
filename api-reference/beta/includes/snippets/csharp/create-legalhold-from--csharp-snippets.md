---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new LegalHold
{
	@odata.type = "#microsoft.graph.ediscovery.legalHold",
	Description = "String",
	CreatedBy = new IdentitySet
	{
		@odata.type = "microsoft.graph.identitySet",
	},
	IsEnabled = "Boolean",
	Status = "String",
	ContentQuery = "String",
	Errors = new List<String>
	{
		"String",
	}
	DisplayName = "String",
};
var result = await graphClient.Compliance.Ediscovery.Cases["case-id"].LegalHolds.PostAsync(requestBody);


```