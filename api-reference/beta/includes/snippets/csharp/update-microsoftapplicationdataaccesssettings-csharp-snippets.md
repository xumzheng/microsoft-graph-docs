---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new MicrosoftApplicationDataAccessSettings
{
	DisabledForGroup = "edbfe4fb-ec70-4300-928f-dbb2ae86c981",
};
await graphClient.Organization["organization-id"].Settings.MicrosoftApplicationDataAccess.PatchAsync(requestBody);


```