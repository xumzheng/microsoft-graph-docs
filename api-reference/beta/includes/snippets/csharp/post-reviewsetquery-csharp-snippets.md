---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ReviewSetQuery
{
	DisplayName = "My Query 1",
	Query = "(subject:\"Quarterly Financials\")",
};
var result = await graphClient.Compliance.Ediscovery.Cases["case-id"].ReviewSets["reviewSet-id"].Queries.PostAsync(requestBody);


```