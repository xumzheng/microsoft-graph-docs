---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.DeviceManagement.VirtualEndpoint.CloudPCs.Item.MicrosoftGraphChangeUserAccountType.ChangeUserAccountTypePostRequestBody
{
	UserAccountType = CloudPcUserAccountType.Administrator,
};
await graphClient.DeviceManagement.VirtualEndpoint.CloudPCs["cloudPC-id"].MicrosoftGraphChangeUserAccountType.PostAsync(requestBody);


```