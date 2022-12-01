---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new SecureScoreControlProfile
{
	ControlStateUpdates = "controlStateUpdates-value",
};
var result = await graphClient.Security.SecureScoreControlProfiles["secureScoreControlProfile-id"].PatchAsync(requestBody);


```