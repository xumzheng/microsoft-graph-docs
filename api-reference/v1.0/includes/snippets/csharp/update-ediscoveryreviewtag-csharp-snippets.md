---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new EdiscoveryReviewTag
{
	DisplayName = "My tag API 2",
	Description = "Use Graph API to create tags (updated)",
};
await graphClient.Security.Cases.EdiscoveryCases["ediscoveryCase-id"].Tags["ediscoveryReviewTag-id"].PatchAsync(requestBody);


```