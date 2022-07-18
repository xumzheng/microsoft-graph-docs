---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new UpdateAudienceRequestBody
{
	AddMembers = new List<Object>
	{
		new 
		{
			AdditionalData = new()
			{
				{"@odata.type", "#microsoft.graph.windowsUpdates.azureADDevice"},
				{"id", "String (identifier)"},
			}
		},
	}
	RemoveMembers = new List<Object>
	{
		new 
		{
			AdditionalData = new()
			{
				{"@odata.type", "#microsoft.graph.windowsUpdates.azureADDevice"},
				{"id", "String (identifier)"},
			}
		},
	}
	AddExclusions = new List<Object>
	{
		new 
		{
			AdditionalData = new()
			{
				{"@odata.type", "#microsoft.graph.windowsUpdates.azureADDevice"},
				{"id", "String (identifier)"},
			}
		},
	}
	RemoveExclusions = new List<Object>
	{
		new 
		{
			AdditionalData = new()
			{
				{"@odata.type", "#microsoft.graph.windowsUpdates.azureADDevice"},
				{"id", "String (identifier)"},
			}
		},
	}
};
await graphClient.Admin.Windows.Updates.Deployments["deployment-id"].Audience.UpdateAudience.PostAsync(requestBody);


```