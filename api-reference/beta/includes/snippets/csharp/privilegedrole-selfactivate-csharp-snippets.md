---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.PrivilegedRoles.Item.MicrosoftGraphSelfActivate.SelfActivatePostRequestBody
{
	Reason = "reason-value",
	Duration = "duration-value",
	TicketNumber = "ticketNumber-value",
	TicketSystem = "ticketSystem-value",
};
var result = await graphClient.PrivilegedRoles["privilegedRole-id"].MicrosoftGraphSelfActivate.PostAsync(requestBody);


```