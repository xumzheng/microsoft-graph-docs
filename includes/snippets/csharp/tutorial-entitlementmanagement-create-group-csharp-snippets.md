---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Group
{
	Description = "Marketing group",
	DisplayName = "Marketing resources",
	MailEnabled = false,
	MailNickname = "markres",
	SecurityEnabled = true,
};
var result = await graphClient.Groups.PostAsync(requestBody);


```