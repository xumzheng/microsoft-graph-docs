---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta..IdentityGovernance.LifecycleManagementSettings
{
	WorkflowScheduleIntervalInHours = 3,
	AdditionalData = new Dictionary<string, object>
	{
		{
			"@odata.context" , "https://graph.microsoft.com/beta/$metadata#identityGovernance/lifecycleWorkflows/settings/$entity"
		},
	},
};
await graphClient.IdentityGovernance.LifecycleWorkflows.Settings.PatchAsync(requestBody);


```