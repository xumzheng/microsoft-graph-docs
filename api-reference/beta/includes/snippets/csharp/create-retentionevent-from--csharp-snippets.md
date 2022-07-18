---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new RetentionEvent
{
	@odata.type = "#microsoft.graph.security.retentionEvent",
	DisplayName = "String",
	Description = "String",
	EventQueries = new List<EventQuery>
	{
		new EventQuery
		{
			AdditionalData = new()
			{
				{"@odata.type", "microsoft.graph.security.eventQueries"},
			}
		},
	}
	EventTriggerDateTime = DateTimeOffset.Parse("String (timestamp)"),
	CreatedBy = new IdentitySet
	{
		@odata.type = "microsoft.graph.identitySet",
	},
	EventPropagationResults = new List<EventPropagationResult>
	{
		new EventPropagationResult
		{
			AdditionalData = new()
			{
				{"@odata.type", "microsoft.graph.security.eventPropagationResult"},
			}
		},
	}
	EventStatus = new RetentionEventStatus
	{
		AdditionalData = new()
		{
			{"@odata.type", "microsoft.graph.security.retentionEventStatus"},
		}
	},
	LastStatusUpdateDateTime = DateTimeOffset.Parse("String (timestamp)"),
};
var result = await graphClient.Security.Triggers.RetentionEvents.PostAsync(requestBody);


```