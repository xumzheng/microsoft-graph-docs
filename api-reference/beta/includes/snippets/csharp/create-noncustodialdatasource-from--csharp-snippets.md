---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new NoncustodialSource
{
	AdditionalData = new Dictionary<string, object>
	{
		{
			"@odata.id" , "https://canary.graph.microsoft.com/testprodbetancsdsaslist/compliance/ediscovery/cases/06d52284-ed81-49b8-904a-b863d3164731/noncustodialDataSources/39383530323537383742433232433246"
		},
	},
};
await graphClient.Compliance.Ediscovery.Cases["case-id"].SourceCollections["sourceCollection-id"].NoncustodialSources["noncustodialDataSource-id"].PostAsync(requestBody);


```