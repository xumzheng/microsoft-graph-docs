---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Models.Security.EdiscoveryCase
{
	DisplayName = "CONTOSO LITIGATION-005",
	Description = "Project Bazooka",
	ExternalId = "324516",
};
var result = await graphClient.Security.Cases.EdiscoveryCases.PostAsync(requestBody);


```