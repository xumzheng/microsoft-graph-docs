---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new CreateLinkPostRequestBody
{
	Type = "edit",
	Scope = "organization",
};
var result = await graphClient.Sites["site-id"].Lists["list-id"].Items["listItem-id"].CreateLink.PostAsync(requestBody);


```