---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new LegalHold
{
	OdataType = "#microsoft.graph.ediscovery.legalHold",
	Description = "String",
	CreatedBy = new IdentitySet
	{
		OdataType = "microsoft.graph.identitySet",
	},
	IsEnabled = boolean,
	Status = LegalHoldStatus.String,
	ContentQuery = "String",
	Errors = new List<>
	{
		"String",
	},
	DisplayName = "String",
};
var result = await graphClient.Compliance.Ediscovery.Cases["case-id"].LegalHolds.PostAsync(requestBody);


```