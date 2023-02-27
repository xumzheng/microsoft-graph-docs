---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.PrivilegedRoleAssignments.Item.MicrosoftGraphMakePermanent.MakePermanentPostRequestBody
{
	Reason = "reason-value",
	TicketNumber = "ticketNumber-value",
	TicketSystem = "ticketSystem-value",
};
var result = await graphClient.PrivilegedRoleAssignments["privilegedRoleAssignment-id"].MicrosoftGraphMakePermanent.PostAsync(requestBody);


```