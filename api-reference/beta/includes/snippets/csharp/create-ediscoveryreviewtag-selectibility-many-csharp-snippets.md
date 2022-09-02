---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new EdiscoveryReviewTag
{
	DisplayName = "My tag API",
	Description = "Use Graph API to create tags",
	ChildSelectability = ChildSelectability.Many,
};
var result = await graphClient.Security.Cases.EdiscoveryCases["ediscoveryCase-id"].Tags.PostAsync(requestBody);


```