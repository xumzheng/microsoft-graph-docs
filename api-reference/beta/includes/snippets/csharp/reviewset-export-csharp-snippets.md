---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ExportRequestBody
{
	OutputName = "2020-12-06 Contoso investigation export",
	Description = "Export for the Contoso investigation",
	ExportOptions = "originalFiles,fileInfo,tags",
	ExportStructure = "directory",
};
await graphClient.Compliance.Ediscovery.Cases["case-id"].ReviewSets["reviewSet-id"].Export.PostAsync(requestBody);


```