---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ItemPatent
{
	Number = "USPTO-3954432633",
	WebUrl = "https://patents.gov/3954432633",
};
await graphClient.Users["user-id"].Profile.Patents["itemPatent-id"].PatchAsync(requestBody);


```