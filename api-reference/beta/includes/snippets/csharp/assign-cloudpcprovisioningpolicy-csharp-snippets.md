---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AssignmentsRequestBody
{
	Assignments = new List<Object>
	{
		new 
		{
			AdditionalData = new()
			{
				{"id", "b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff"},
			}
		},
	}
	AdditionalData = new()
	{
		{"@odata.type", "#microsoft.graph.cloudPcProvisioningPolicyAssignment"},
	}
};
await graphClient.DeviceManagement.VirtualEndpoint.ProvisioningPolicies["cloudPcProvisioningPolicy-id"].Assign.PostAsync(requestBody);


```