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
			"@odata.id" , "https://graph.microsoft.com/beta/security/cases/ediscoveryCases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/noncustodialDataSources/39333641443238353535383731453339"
		},
	},
};
await graphClient.Security.Cases.EdiscoveryCases["ediscoveryCase-id"].Searches["ediscoverySearch-id"].NoncustodialSources["ediscoveryNoncustodialDataSource-id"].PostAsync(requestBody);


```