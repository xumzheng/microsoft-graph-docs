---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

// Code snippets are only available for the latest version. Current version is 5.x

var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.PrivilegedRoles.Item.SelfActivate.SelfActivatePostRequestBody
{
	Reason = "reason-value",
	Duration = "duration-value",
	TicketNumber = "ticketNumber-value",
	TicketSystem = "ticketSystem-value",
};
var result = await graphClient.PrivilegedRoles["{privilegedRole-id}"].SelfActivate.PostAsync(requestBody);


```