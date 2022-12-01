---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Organization.Item.ActivateService.ActivateServicePostRequestBody
{
	SkuId = "6fd2c87f-b296-42f0-b197-1e91e994b900",
	ServicePlanId = "a23b959c-7ce8-4e57-9140-b90eb88a9e97",
};
await graphClient.Organization["organization-id"].ActivateService.PostAsync(requestBody);


```