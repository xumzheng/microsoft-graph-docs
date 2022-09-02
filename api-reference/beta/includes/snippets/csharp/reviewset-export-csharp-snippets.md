---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Compliance.Ediscovery.Cases.Item.ReviewSets.Item.Export.ExportPostRequestBody
{
	OutputName = "2020-12-06 Contoso investigation export",
	Description = "Export for the Contoso investigation",
	ExportOptions = Microsoft.Graph.Beta.Models.Ediscovery.ExportOptions.OriginalFiles | Microsoft.Graph.Beta.Models.Ediscovery.ExportOptions.FileInfo | Microsoft.Graph.Beta.Models.Ediscovery.ExportOptions.Tags,
	ExportStructure = Microsoft.Graph.Beta.Models.Ediscovery.ExportFileStructure.Directory,
};
await graphClient.Compliance.Ediscovery.Cases["case-id"].ReviewSets["reviewSet-id"].Export.PostAsync(requestBody);


```