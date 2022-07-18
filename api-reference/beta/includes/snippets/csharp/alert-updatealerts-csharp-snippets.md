---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ValueRequestBody
{
	Value = new List<Object>
	{
		new 
		{
			AdditionalData = new()
			{
				{"assignedTo", "String"},
				{"closedDateTime", "String (timestamp)"},
				{"comments", new List<String>
				{
					"String",
				}
				{"id", "String (identifier)"},
				{"tags", new List<String>
				{
					"String",
				}
			}
		},
	}
};
var result = await graphClient.Security.Alerts.UpdateAlerts.PostAsync(requestBody);


```