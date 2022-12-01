---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Communications.Calls.Item.ChangeScreenSharingRole.ChangeScreenSharingRolePostRequestBody
{
	Role = ScreenSharingRole.Viewer,
};
await graphClient.Communications.Calls["call-id"].ChangeScreenSharingRole.PostAsync(requestBody);


```