---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Security.Cases.EdiscoveryCases.Item.ReviewSets.Item.Export.ExportPostRequestBody
{
	OutputName = "Export via API",
	Description = "Export for the Contoso investigation",
	ExportOptions = ExportOptions.Originalfiles,fileinfo,tags,
	ExportStructure = ExportFileStructure.Directory,
};
await graphClient.Security.Cases.EdiscoveryCases["ediscoveryCase-id"].ReviewSets["ediscoveryReviewSet-id"].Export.PostAsync(requestBody);


```