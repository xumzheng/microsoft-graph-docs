---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.DeviceManagement.VirtualEndpoint.CrossCloudGovernmentOrganizationMapping.CrossCloudGovernmentOrganizationMappingPostRequestBody
{
};
await graphClient.DeviceManagement.VirtualEndpoint.CrossCloudGovernmentOrganizationMapping.PostAsync(requestBody, (requestConfiguration) =>
{
	requestConfiguration.Headers.Add("X-MS-CloudPC-USGovCloudTenantAADToken", "{token}");
});


```